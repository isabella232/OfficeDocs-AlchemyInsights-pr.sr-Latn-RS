---
title: 1491-search-not-returning-expected-results
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
- "1491"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: 846034d68a59d053cbe37aeba3a75e20a60786fd7ff24106964229b1deb77608
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "54052724"
---
# <a name="content-search-not-returning-expected-results"></a>Pretraga sadržaja ne daje očekivane rezultate

Prilikom pokretanje pretraga sadržaja iz Microsoft 365 centra za & usaglašenost, možda ćete dobiti neočekivane rezultate pretrage. Razmotrite sledeće stvari koje mogu da utiču na rezultate pretrage:

- **Lokacije sadržaja i uslovi pretrage:** Uverite se da ste izabrali odgovarajuće lokacije sadržaja i uslove pretrage. Ako ste vodili veliku pretragu (sa mnogo lokacija), razmislite o tome da je podelite na više pretraga.

- **Delimično indeksirane stavke:**  [Delimično indeksirane stavke](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) iz poštančkih sandučića su uključene u procenjene rezultate pretrage. Međutim, delimično indeksirane stavke sa SharePoint i OneDrive nisu uključene u procenu pretrage.

- Neuspele pretrage: Prilikom pretraživanja velikog broja poštanskih sandučića (preko 100.000 poštanskog sandučića), možete dobiti greške u pretrazi sa kodovima grešaka kao što su CS008-009 i CS012-002). U ovom slučaju, ponovo potražite samo lokacije sadržaja koje nisu uspele. Više  [informacija potražite u](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) ovom članku.
