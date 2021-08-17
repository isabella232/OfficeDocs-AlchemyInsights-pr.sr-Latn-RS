---
title: 1490-rešavanje problema-eDiscovery-failures
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1490"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: 7b819b9bb18b5c0a635e708eccc0f23271267874707e5f3a7d41b633a05f2822
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "54105582"
---
# <a name="troubleshoot-content-search-errors"></a>Rešavanje problema sa greškama u pretrazi sadržaja

Da li nailazite na probleme sa pretragom sadržaja ili nailazite na neuspeh prilikom izvoza rezultata pretrage?

Na primer, da li dobijate sledeće prilikom pretraživanja?

- CS008 ili CS012 greške

- Greške zauzetosti/vremenskog perioda servera

- Došlo je do greške u aplikaciji

Ili prilikom pretrage ili izvoza rezultata iz velikog broja poštannih sandučića (preko 100.000 poštanskog sandučića), dobijate greške u izvozu?

Za ove tipove grešaka, ponovo potražite lokacije sadržaja koje nisu uspele. Više  [informacija potražite u](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) ovom članku.

Ako izvozite više od 100K poštannih sandučića, biće potrebno da koristite sledeći PowerShell da biste preuzeli rezultate izvoza: Izvoz rezultata iz više od  [100K](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes)poštannih sandučića.
