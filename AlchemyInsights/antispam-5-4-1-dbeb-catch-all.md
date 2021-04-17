---
title: AntiSpam 5.4.1 DBEB catch-all
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001209"
- "3167"
ms.openlocfilehash: c6ce26a133428dc7351912d8250ef096dfc7521a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821461"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a>Rešavanje problema sa isporukom za kôd greške 550 5.4.1 Relay Access Denied

Do ovog problema dolazi prilikom [provere da li](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) je e-adresa važeća za sprečavanje povratnih grešaka prilikom ulaska na Microsoft mrežu. Pokušajte sledeće:

1. Utvrdite da li je problem specifičan za ceo domen ili za jednu e-adresu:
    - Ceo domen: Domen ponekad treba da se sinhronizuje; pokušajte [da podešavanje domena na Interni, a zatim se vratite na ovlašćeni](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).
    - Jedna adresa e-pošte: Ponekad adresa treba da se sinhronizuje; promena smtp proxy adrese, a zatim promena nazad može pomoći.
2. Utvrdite da li je problem specifičan za grupu ili javnu fasciklu. Za neke tipove objekata ćete možda morati ručno da kreirate u Azure Active Directory.

Ako vam je potrebna dodatna pomoć, otvorite tiket za podršku i navedite polje problema (uključujući tip objekta na koji šaljete) kako bismo vam pomogli bolje.