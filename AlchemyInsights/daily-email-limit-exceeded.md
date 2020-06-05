---
title: Premašen je dnevni limit e-pošte. Tok posla je obustavljen.
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: 701c4aef6bfc0c4a2c4570f6dd16dbe4f99efc44
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580347"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a>Premašen je dnevni limit e-pošte. Tok posla je obustavljen.

Ova greška može biti primljena u sledećim slučajevima:

- Imate tok posla na SharePoint mreži koji koristi tip platforme SharePoint 2010 ili SharePoint 2013 Workflow.
- Tok posla je konfigurisan da šalje prilagođenu e-poruku u više od 200 korisnika u isto vreme, više od 10.000 primalaca dnevno ili više od 30 poruka u minuti.
- Kada pokrenete tok posla, e-poruka se ne šalje i primetićete sledeće ponašanje:
    - Za tok posla koji koristi tip SharePoint 2013 platforme, potražite stranicu " **Status toka posla** ". Na stranici "Status toka posla", **unutrašnji status** je postavljen na " **pokrenuto**", a "informacioni balon" **ne može da pošalje primaocu**.

Da biste zaobišli ovaj problem, konfigurišite tok posla za slanje e-poruka bez prekoračenja [ograničenja za Exchange online](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits). Na primer, koristite pauzu u toku posla, pošaljite e-poruku u Microsoft 365 grupu, grupu za distribuciju ili bezbednosnu grupu za koju je omogućena pošta ili pošaljite poruku na manje od 200 primalaca.


Više informacija potražite u sledećem [članku](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).

## <a name="related-topics"></a>Povezane teme
- [Kreiraj tok](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint i protok](https://flow.microsoft.com/blog/sharepoint-and-flow/) 