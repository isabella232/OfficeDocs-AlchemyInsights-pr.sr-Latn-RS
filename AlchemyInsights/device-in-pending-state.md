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
ms.openlocfilehash: f70b43a8b914b0d2dda9db61606b8ae24523f869
ms.sourcegitcommit: 097a8cabe0d2280af489159789988a0ab532dabb
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 12/11/2020
ms.locfileid: "49679990"
---
# <a name="device-in-pending-state"></a>Uređaj u stanju čekanja

**Preduslovi**

1. Ako podešavate registraciju uređaja po prvi put, uverite se da ste redigovali [Uvod u upravljanje uređajima u usluzi Azure Active Directory (AZURE AD)](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support) koji će vas voditi na način na koji se uređaji mogu kontrolisati u kontroli Azure AD.
2. Ako registraciju uređaja u Azure AD registrujete direktno i unosite ih u Intune, moraćete da proverite da li ste prvo [konfigurisali Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) i da imaju [licenciranje](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) .
3. Uverite se da ste ovlašćeni za obavljanje operacija u usluzi Azure AD i lokalnoj REKLAMI. Samo globalni administrator u usluzi Azure AD može da upravlja postavkama za registraciju uređaja. Pored toga, ako podešavate automatske registracije u lokalnom aktivnom direktorijumu, moraćete da budete administrator aktivnog direktorijuma i AD FS (ako je primenljivo).

Hibridni Azure AD pridruži se sistemu za registraciju zahteva uređaje za korporativnu mrežu. Radi i preko VPN mreže, ali u tome ima nekih problema. Čuli smo da klijenti trebaju pomoć za rešavanje problema sa procesom registracije hibridnog Azure AD.

**Okruženje za potvrdu identiteta u oblaku (pomoću hash sinhronizacije Azure oglasa lozinki ili prosleрenog identiteta)**

Ovaj tok registracije je poznat i kao "Pridruživanje sastanku".

Evo šta se dešava tokom procesa registracije:

1. Windows 10 otkriva zapis povezivanja usluge (SCP) kada se korisnik prijavi na uređaj.

    1. Uređaj prvi put pokušava da preuzme informacije o zakupcu iz klijenta u registratoru, [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD]. Više informacija potražite u članku [dokument](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).
    1. Ako ne uspe, uređaj komunicira sa lokalnim aktivnim direktorijumom da bi dobio informacije o zakupcu iz SCP. Da biste potvrdili SCP, uputite ovaj [dokument](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point).

    > [!NOTE]
    > Preporučujemo omogućavanje SCP-a u aktivnom direktorijumu i samo pomoću dodatka za podešavanje početne validacije.

2. Windows 10 pokušava da komunicira sa uslugom Azure AD u okviru konteksta sistema da bi se potvrdio na osnovu Azure AD.

    Možete da proverite da li uređaj može da pristupi Microsoft resursima u okviru sistemskog naloga pomoću [skripata za povezivanje registracije uređaja](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0).

3. Windows 10 generiše samopotpisani certifikat i skladišti ga ispod objekta računara u lokalnoj aktivnoj fascikli. Ovo zahteva liniju vida na kontroler domena.

4. Objekat uređaja koji ima certifikat sinhronizovan je sa lokacijom Azure AD putem Azure AD Connect. Ciklus sinhronizacije je podrazumevano svakih 30 minuta, ali to zavisi od konfiguracije Azure AD Connect. Više informacija potražite u [dokumentu](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).

5. U ovoj fazi, trebalo bi da možete da vidite uređaj tema "**Neobrađeno**" u okviru "oљtrica device" Azure portala.

6. Na sledećoj prijavi korisnika na Windows 10, registracija će biti dovršena.

    > [!NOTE]
    > Ako ste na VPN-u i odjavljivanje/prijava prekida vezu ka domenu, možete ručno pokrenuti registraciju. Da biste to uradili:
    >
    > Izdaju `dsregcmd /join` lokalno za administratorski odziv ili daljinski pomoću usluge PSExec na računar.
    >
    > Na primer: `PsExec -s \\win10client01 cmd, dsregcmd /join`

Za uobičajene probleme sa sistemom Azure Active Directory, pogledajte [najčešća pitanja o uređajima](https://docs.microsoft.com/azure/active-directory/devices/faq).
