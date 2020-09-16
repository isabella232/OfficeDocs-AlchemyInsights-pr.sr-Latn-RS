---
title: 1491-rezultati
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
ms.openlocfilehash: 5c4452726c1dbe2232ee63e8a9ee4d089f5c76db
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47740488"
---
# <a name="content-search-not-returning-expected-results"></a>Pretraga sadržaja ne vraća očekivane rezultate

Prilikom pokretanja Pretraga sadržaja iz Microsoft 365 Security & centra za usaglašenost, možda ćete dobiti neočekivane rezultate pretrage. Razmotrite sledeće stvari koje mogu da utiču na rezultate pretrage:

- **Lokacije sadržaja i uslovi pretrage**: uverite se da ste izabrali odgovarajuće lokacije sadržaja i uslove pretrage. Ako ste pokrenuli veliku pretragu (sa mnogo lokacija), razmotrite da je razdelite u više pretraga.

- **Delimično indeksirane stavke**:  [delimično indeksirane](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) stavke iz poštanskog sandučića obuhvaćene su procenjenim rezultatima pretrage. Međutim, delimično indeksirane stavke sa lokacija u sistemu SharePoint i OneDrive nisu uključene u procenu pretrage.

- **Otkazivanja pretrage**: kada pretražujete veliki broj poštanskih sandučića (preko 100.000 poštanskih sandučića), možete da dobijete greške prilikom pretrage sa kodom greške kao što su CS008-009 i CS012-002). U ovom slučaju ponovo pokušajte da izvršite pretragu samo za lokacije koje nisu uspele. Više informacija potražite u  [članku ovaj članak](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) .
