---
title: Rešavanje problema sa PRT-om
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/01/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000076"
- "7317"
ms.openlocfilehash: fd285d1158d7b358e4c698cf6014422cc2fb536e1fbdf98630bebda359f9c553
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "53972730"
---
# <a name="troubleshoot-prt-issue"></a>Rešavanje problema sa PRT-om

Da bi se dovršila potvrda identiteta za bilo koji uređaj, on mora biti potpuno registrovan i u dobrom stanju i može da nabavi primarni token za osvežavanje (PRT).

Proces registracije hibridne usluge Azure AD zahteva da uređaji budu na korporativnoj mreži. On takođe funkcioniše preko VPN-a, ali za to postoje neke pećine. Čuli smo da klijentima treba pomoć za rešavanje problema hibridnog procesa registracije Azure AD pridruživanja u udaljenim okolnostima. Evo potvrde onoga što se dešava "ispod haube" tokom procesa registracije.

**Okruženje potvrde identiteta u oblaku (pomoću sinhronizacije sinhronizacije i prolazne potvrde identiteta za Azure AD lozinke)**

Ovaj tok registracije je poznat i kao "Sinhronizuj spajanje".

1. Windows 10 otkrije SCP zapis kada se korisnik prijavi na uređaj.
    1. Uređaj prvo pokušava da preuzme informacije o zakupcu sa SCP-a klijenta u registratoru [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD]. Dodatne informacije potražite u ovom [dokumentu.](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control)
    2. Ako ne uspe, uređaj komunicira sa uslugom Active Directory (AD) u cilju dobijanja informacija o zakupcu iz usluge Connection Point (SCP). Da biste potvrdili SCP, pogledajte ovaj [dokument.](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point) 

> [!NOTE]
> Preporučujemo da omogućavate SCP u AD-u i da koristite samo SCP na strani klijenta za početnu proveru valjanosti.

2. Windows 10 da komunicira sa uslugom Azure AD u okviru konteksta sistema da bi se potvrdio identitet u Azure AD. Možete da proverite da li uređaj može da pristupi Microsoft resursima u okviru naloga sistema pomoću skripte probne registracije uređaja.

3. Windows 10 generiše samo potpisani certifikat i skladišti ga u okviru objekta računara u lokalnoj OD-u. Ovo zahteva kontroluer domena na vidnom mestu.

4. Objekat uređaja koji ima certifikat sinhronizuje se sa Azure AD putem Azure AD Povezivanje. Ciklus sinhronizacije podrazumevano je svakih 30 minuta, ali zavisi od konfiguracije Azure AD Povezivanje. Dodatne informacije potražite u ovom [dokumentu.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering)

5. U ovom trenutku bi trebalo da možete da vidite uređaj za temu u stanju "Na čekanju" u okviru Blejd uređaja Azure portala.

6. Kada se sledeći korisnik prijavi Windows 10, registracija će biti dovršena. 

> [!NOTE]
> Ako ste na VPN-u, a proces prijavljivanja logotipom obustavljuje povezivanje domena, možete ručno da pokrenete registraciju:
 1. Izdajte dsregcmd /pridružite se lokalno na odzivu za adminitražu ili daljinski putem PSExec-a ka računaru. Na primer, PsExec -s \\ win10client01 cmd, dsregcmd /join

 2. Više detalja o problemima sa hibridnim spajanjem pogledajte u odeljku [Rešavanje problema sa uređajima.](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/azure-ad-mailbag-frequent-questions-about-using-device-based/ba-p/1257344)
