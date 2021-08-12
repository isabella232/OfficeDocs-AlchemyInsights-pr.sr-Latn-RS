---
title: Problemi sa performansama SharePoint ili OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1133"
- "2397"
- "2418"
- "5200018"
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 921aae7eba8487c5600f290fd671ef2675372e6af0478b913e38354856cbaa22
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "53911856"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint ili OneDrive sporim, nedostupnim ili nedostupnim za više korisnika

SharePoint ili OneDrive mogu da budu spore, nedostupne ili nedostupne ili mogu da prikažu uslugu koja nije dostupna ili 503 greške iz nekoliko razloga:
  
- Ako je SharePoint ili OneDrive sajt spor ili odložen za više korisnika, možda postoji privremeni problem sa uslugom gde korisnici nailaziju na povremena kašnjenja ili greške u navigaciji prilikom pristupa SharePoint lokacijama OneDrive sadržaju. Proverite [kontrolnu tablu Za zdravstveno stanje usluge](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) da biste videli da li to utiče na vašu organizaciju.
  
- Korisnici mogu da dobiju *grešku "503 server* je zauzet" kada pokušavaju da odu na SharePoint ili OneDrive sajtove. Do ove greške može da SharePoint usluge. SharePoint Online koristi ograničavanje da bi održao optimalne performanse i pouzdanost usluge SharePoint Online. Ograničavanje ograničava broj korisničkih radnji ili istovremenih poziva (po skripti ili kodu) kako bi se sprečilo prekomerno korišćenje resursa. Dodatne informacije o zabrani potražite u temi Izbegavanje relacije ili [blokiranja u SharePoint Online.](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)

- Ako naiđete  na spore performanse sa klasičnim ili [](https://aka.ms/perftool) **modernim** SharePoint sajtom ili stranicom, utisku alatke "Dijagnostika stranice" za analiziranje stranica.
  
- Ako i dalje imate uopštene spore performanse, pregledajte resurse na dnu ovog članka: Uvod u podučavanje performansi za [SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334)
  