---
title: Uređaj u stanju čekanja
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003244"
- "7319"
ms.openlocfilehash: 224e6e613c306b50e354930bcbe6f43f1c08528766cb6e681b0e9826b2d55a4d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "53914017"
---
# <a name="device-in-pending-state"></a>Uređaj u stanju čekanja

**Preduslovi:**

1. Ako po prvi put postavljate registracije uređaja, uverite se da ste pregledali Uvod u upravljanje uređajima u Azure Active Directory [(Azure AD)](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support) koji će vas voditi kroz to kako da nabavite uređaje pod kontrolom sistema Azure AD.
2. Ako direktno registrujete uređaje u uslugu Azure AD i upisujete ih u [Intune,](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) morate [](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) da se uverite da ste konfigurisali Intune i da prvo imate licenciranje na mestu.
3. Uverite se da ste ovlašćeni za izvršavanje operacija u uslugama Azure AD i na sajtu AD. Postavkama za registracije uređaja može da upravlja samo globalni administrator u usluzi Azure AD. Pored toga, ako podešavate automatske registracije u lokalnom aktivnom direktorijumu, moraćete da budete administrator za aktivni direktorijum i AD FS (ako je primenljivo).

Proces registracije hibridne usluge Azure AD zahteva da uređaji budu na korporativnoj mreži. On takođe funkcioniše preko VPN-a, ali za to postoje neke pećine. Čuli smo da klijentima treba pomoć za rešavanje problema hibridnog procesa registracije Azure AD pridruživanja u udaljenim radnim okolnostima.

**Okruženje potvrde identiteta u oblaku (pomoću sinhronizacije sinhronizacije i prolazne potvrde identiteta za Azure AD lozinke)**

Ovaj tok registracije je poznat i kao "Sinhronizuj spajanje".

Evo sloma onoga što se događa tokom procesa registracije:

1. Windows 10 zapis tačke povezivanja usluge (SCP) kada se korisnik prijavi na uređaj.

    1. Uređaj prvo pokušava da preuzme informacije o zakupcu sa SCP-a klijenta u registratoru [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD]. Dodatne informacije potražite u [dokumentu](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).
    1. Ako ne uspe, uređaj komunicira sa kompanijom Active Directory u cilju dobijanja informacija o zakupcu iz SCP-a. Da biste potvrdili SCP, pogledajte [ovaj dokument.](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point)

    > [!NOTE]
    > Preporučujemo da omogućavate SCP u aktivnom direktorijumu i da koristite SCP na strani klijenta samo za početnu proveru valjanosti.

2. Windows 10 da komunicira sa uslugom Azure AD u okviru konteksta sistema da bi se potvrdio identitet u Azure AD.

    Možete da proverite da li uređaj može da pristupi Microsoft resursima u okviru naloga sistema pomoću skripte [za testiranje](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0)povezivanja uređaja.

3. Windows 10 generiše samo potpisani certifikat i skladišti ga u okviru objekta računara u lokalnoj službi Active Directory. Ovo zahteva kontroluer domena na vidnom mestu.

4. Objekat uređaja koji ima certifikat sinhronizuje se sa Azure AD putem Azure AD Povezivanje. Ciklus sinhronizacije podrazumevano je svakih 30 minuta, ali zavisi od konfiguracije Azure AD Povezivanje. Dodatne informacije potražite u ovom [dokumentu.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering)

5. U ovom trenutku bi trebalo da možete da vidite uređaj za temu u stanju **"Na** čekanju" u okviru Blejd uređaja Azure portala.

6. Kada se sledeći korisnik prijavi Windows 10, registracija će biti dovršena.

    > [!NOTE]
    > Ako ste na VPN-u, a logotip/prijavljivanje obustavljuje povezivanje domena, možete ručno da pokrenete registraciju. Da biste to uraditi:
    >
    > Lokalno `dsregcmd /join` na odzivu za adminis, ili daljinski putem usluge PSExec na računaru.
    >
    > Na primer: `PsExec -s \\win10client01 cmd, dsregcmd /join`

Za uobičajene probleme sa registracijom Azure Active Directory uređaja, pogledajte najčešća [pitanja o uređajima.](https://docs.microsoft.com/azure/active-directory/devices/faq)
