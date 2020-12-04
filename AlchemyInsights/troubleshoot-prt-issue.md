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
ms.openlocfilehash: 8e654a38d720aa51daf21bf5c3fb0da8b9c3d8e7
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573725"
---
# <a name="troubleshoot-prt-issue"></a>Rešavanje problema sa PRT-om

Da bi bilo koji uređaj mogao da se dovrši, mora da bude potpuno registrovan i u dobroj državi i da može da pribavi primarni Token osvežavanja (PRT).

Hibridni Azure AD pridruži se sistemu za registraciju zahteva uređaje za korporativnu mrežu. Radi i preko VPN mreže, ali u tome ima nekih problema. Čuli smo da klijenti treba da imaju pomoć za rešavanje problema sa operativnim sistemom Azure AD se pridruži registraciji u okviru okolnosti sa udaljenog posla. Evo šta se dešava, tokom procesa registracije.

**Okruženje za potvrdu identiteta u oblaku (pomoću hash sinhronizacije Azure oglasa lozinki ili prosleрenog identiteta)**

Ovaj tok registracije je poznat i kao "Pridruživanje sastanku".

1. Windows 10 otkriva SCP zapis po prijavljivanju korisnika na uređaj.
    1. Uređaj prvi put pokušava da preuzme informacije o zakupcu iz klijenta u registratoru, [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD]. Više informacija potražite u članku ovaj [dokument](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control).
    2. Ako ne uspe, uređaj komunicira sa lokalnim aktivnim direktorijumom (AD) da biste dobili informacije o zakupcu iz tačaka povezivanja usluge (SCP). Da biste potvrdili SCP, pogledajte ovaj [dokument](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point). 

> [!NOTE]
> Preporučujemo omogućavanje SCP-a u OGLASU i samo pomoću dodatka za početnu validaciju.

2. Windows 10 pokušava da komunicira sa uslugom Azure AD u okviru konteksta sistema da bi se potvrdio na osnovu Azure AD. Možete da proverite da li uređaj može da pristupi Microsoft resursima u okviru sistemskog naloga pomoću skripata za povezivanje registracije uređaja.

3. Windows 10 generiše samopotpisani certifikat i skladišti ga ispod objekta računara u lokalnoj REKLAMI. Ovo zahteva liniju vida na kontroler domena.

4. Objekat uređaja koji ima certifikat se sinhronizuje na Azure AD u usluzi Azure AD Connect. Ciklus sinhronizacije je podrazumevano svakih 30 minuta, ali to zavisi od konfiguracije usluge Azure AD Connect. Za više informacija pogledajte ovaj [dokument](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering).

5. U ovoj fazi, trebalo bi da možete da vidite uređaj tema "Neobrađeno" u okviru "oљtrica device" Azure portala.

6. Na sledećoj prijavi korisnika na Windows 10, registracija će biti dovršena. 

> [!NOTE]
> Ako ste na VPN-u, a proces prijavljivanja prekida povezivanje, možete ručno pokrenuti registraciju:
 1. Izdate dsregcmd/JOIN lokalno u okviru odziv administratora ili daljinski pomoću PSExec na PC računaru. Na primer, PsExec-s \\ win10client01 cmd, dsregcmd/JOIN

 2. Više detalja o problemima sa hibridom pridruživanja potražite u članku [Rešavanje problema sa uređajima](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/azure-ad-mailbag-frequent-questions-about-using-device-based/ba-p/1257344).
