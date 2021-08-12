---
title: Premašen je dnevni limit e-pošte. Tok posla je obustavljen.
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: 60ddbe68298e998a4e0b271a15209efc135c80638702c98dbcb3e0b2f1554860
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "53914665"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a>Premašen je dnevni limit e-pošte. Tok posla je obustavljen.

Ova greška može biti primljena u sledećim scenarijima:

- Imate tok posla u SharePoint Online koji koristi tip SharePoint 2010 ili SharePoint 2013 platforme toka posla.
- Tok posla je konfigurisan tako da šalje prilagođenu e-poruku za više od 200 korisnika istovremeno, više od 10.000 primalaca dnevno ili više od 30 poruka u minutu.
- Kada pokrenete tok posla, e-poruka se ne šalje i primećujete sledeće ponašanje:
    - Za tok posla koji koristi SharePoint 2013 platformi, možete da odete na stranicu **"Status toka posla".** Na stranici "Status toka posla" **status** interne postavke je postavljen na "Pokrenuto", a balon za informacije prikazuje tekst Nije moguće poslati **primaocu.**

Da biste rešili ovaj problem, konfigurišite tok posla tako da šalje e-poruke bez [Exchange Online ograničenja pošiljaoca](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits). Na primer, koristite pauzu u toku posla, pošaljite e-poruku Microsoft 365 grupi, grupi za distribuciju ili bezbednosnoj grupi sa omogućenom poštom ili pošaljite poruku za manje od 200 primalaca istovremeno.


Dodatne informacije potražite u sledećem [članku.](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or)

## <a name="related-topics"></a>Сродне теме
- [Kreiranje Flow](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint i Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 