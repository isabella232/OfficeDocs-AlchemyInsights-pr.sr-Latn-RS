---
title: Brisanje timova privatni kanal
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3781"
- "9001223"
ms.openlocfilehash: 2ee998f0c70973645c273a2a6609af2420a4f74b
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439916"
---
# <a name="delete-a-teams-private-channel"></a>Brisanje timova privatni kanal

Microsoft je svestan problema koji će izbrisati privatni kanal timova ako imate omogućenu SharePoint smernice za zadržavanje za osnovnu SharePoint lokaciju. Microsoft radi na ispravu. U međuvremenu, možete da koristite sledeća rešenja za brisanje privatnog kanala.

**Izuzmite tim/kolekciju lokacija iz SharePoint smernica za zadržavanje.**

1. Posetite Office 365 admin portal i u levom oknu za navigaciju izaberite stavku " **Prikaži sve** ".
2. U okviru opcije " **admin centri**" Idite na **bezbednosnu &**  >  smernice za**sprečavanje gubitka podataka**  >  **Policy**.
3. Identifikujte sve smernice koje se odnose na SharePoint lokacije i izmenite smernice tako da SharePoint lokacija tima koji sadrži privatni kanal nije uključena u smernice za zadržavanje.
4. Sačuvajte smernice.
    Može da potraje i do 24 sata da bi postavke smernica stupile na snagu.
    Nakon što je lokacija isključena, možete da izbrišete privatni kanal.  
    
***Možda*** ćete moći da izbrišete privatni kanal pomoću Microsoft timova na vašem Android uređaju. 

Za srodne SharePoint informacije pogledajte odeljak [nije moguće izbrisati stavke u sistemu SharePoint Online ili OneDrive za posao](https://docs.microsoft.com/alchemyinsights/retention-policy-ediscovery-hold).