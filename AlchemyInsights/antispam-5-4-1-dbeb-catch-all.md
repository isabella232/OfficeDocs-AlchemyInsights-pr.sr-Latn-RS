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
ms.openlocfilehash: e0e9b4fec0615943227f40043aeed842e8ee556c5916a59f65e79ce121ec9547
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "53932291"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a>Rešavanje problema sa isporukom za kôd greške 550 5.4.1 Relay Access Denied

Do ovog problema dolazi prilikom [provere da li](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) je e-adresa važeća za sprečavanje povratnih grešaka prilikom ulaska na Microsoft mrežu. Pokušajte sledeće:

1. Utvrdite da li je problem specifičan za ceo domen ili za jednu e-adresu:
    - Ceo domen: Domen ponekad treba da se sinhronizuje; pokušajte [da podešavanje domena na Interni, a zatim se vratite na ovlašćeni](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).
    - Jedna adresa e-pošte: Ponekad adresa treba da se sinhronizuje; promena smtp proxy adrese, a zatim promena nazad može pomoći.
2. Utvrdite da li je problem specifičan za grupu ili javnu fasciklu. Za neke tipove objekata će možda biti potrebno da se objekti ručno kreiraju u Azure Active Directory.

Ako vam je potrebna dodatna pomoć, otvorite tiket za podršku i navedite polje problema (uključujući tip objekta na koji šaljete) kako bismo vam pomogli bolje.