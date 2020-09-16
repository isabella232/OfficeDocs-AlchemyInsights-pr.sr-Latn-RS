---
title: Problemi sa performansama – SharePoint ili OneDrive
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
ms.openlocfilehash: 28867b71df5353dcee5cc3361742f10357a0efe1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771915"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint ili OneDrive spori, nedostupni ili nedostupni za više korisnika

SharePoint ili OneDrive mogu biti spori, nedostupni ili nedostupni, ili mogu da prikažu usluge nedostupne ili 503 grešaka, iz nekoliko razloga:
  
- Ako je SharePoint ili OneDrive lokacija spora ili odložena za više korisnika, možda može postojati privremeni problem pri uslugama gde korisnici doživljaju povremene kašnjenja ili greške navigacije prilikom pristupanja SharePoint lokacijama ili OneDrive sadržaju. Pogledajte [kontrolnu tablu zdrave usluge](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) da biste videli da li je vaša organizacija uticala na njih.
  
- Korisnici mogu primati *503 server* imate grešku prilikom pokušaja da se krećete na SharePoint ili OneDrive lokacije. Ova greška može biti izazvana pritiskom na SharePoint usluzi. SharePoint Online koristi ograničavanje da bi održao optimalne performanse i pouzdanost usluge SharePoint Online. Ograničavanje ograničava broj korisničkih radnji ili istovremenih poziva (po skripti ili kodu) kako bi se sprečilo prekomerno korišćenje resursa. Više informacija o [ograničavanju pogledajte u sistemu SharePoint online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)

- Ako doživite spore performanse sa **klasičnom** ili **modernom** SharePoint lokacijom ili stranicama, koristite alatku za [dijagnostiku stranice](https://aka.ms/perftool) da biste analizirali stranice.
  
- Ako i dalje nailazite na opšte spore performanse, pregledajte resurse na dnu ovog članka: [Uvod u podešavanje performansi za SharePoint online](https://go.microsoft.com/fwlink/?linkid=2024334)
  