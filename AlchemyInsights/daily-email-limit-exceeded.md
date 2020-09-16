---
title: Dnevno ograničenje za svakodnevne e-poštu. Tok posla obustavljen.
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
ms.openlocfilehash: dfb42b24f1c2b4b05cb067a82505a6a8b63f277e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47731577"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a>Dnevno ograničenje za svakodnevne e-poštu. Tok posla obustavljen.

Ova greška se može primiti u sledećim slučajevima:

- Imate tok posla u sistemu SharePoint online koji koristi SharePoint 2010 ili SharePoint 2013 tip platforme toka posla.
- Tok posla je konfigurisan da šalje prilagođenu e-poruku za više od 200 korisnika po danu, više od 10.000 primalaca dnevno ili više od 30 poruka u minuti.
- Kada pokrećete tok posla, e-poruka se ne šalje i primetićete sledeće ponašanje:
    - Za tok posla koji koristi SharePoint 2013 platformu, potražite stranicu **Status toka posla** . Na stranici "Status toka posla", **unutrašnji status** je podešen na **Početak**, a balončić sa informacijama **ne može da**se prikaže primaocu.

Da biste rešili ovaj problem, konfigurišite tok posla da šalje e-poruke bez prekoračenja [ograničenja Exchange online pošiljaoca](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits). Na primer, koristite pauzu u toku posla, pošaljite e-poruku Microsoft 365 grupi, grupi za distribuciju ili bezbednosnoj grupi sa omogućenom poštom ili pošaljite poruku manjim od 200 primalaca.


Više informacija potražite u sledećem [članku](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).

## <a name="related-topics"></a>Сродне теме
- [Kreiranje protoka](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint i protok](https://flow.microsoft.com/blog/sharepoint-and-flow/) 