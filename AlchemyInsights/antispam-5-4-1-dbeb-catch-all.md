---
title: AntiSpam 5.4.1 DBEB
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001209"
- "3167"
ms.openlocfilehash: f9d613457ae33dc7e00f20391bbdff029500a123
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47717375"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a>Rešavanje problema sa isporukom za kôd greške 550 5.4.1 pristup relej zabranjen

Do ovog problema dolazi prilikom [provere da biste videli da li je adresa e-pošte važeća da biste sprečili](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) pretplatu prilikom ulaska u Microsoft Network. Isprobajte sledeće:

1. Utvrdite da li je problem karakterističan za ceo domen ili jednu e-adresu:
    - Ceo domen: ponekad domen treba da se sinhronizuje; Pokušajte da [postavite domen na unutrašnju, a zatim na autoritativno](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).
    - Jedinstvena e-adresa: ponekad treba da se sinhronizuje adresa; Promena SMTP proxy adrese, a zatim promena može da pomogne.
2. Utvrdite da li je problem karakterističan za grupu ili javnu fasciklu. Za neke tipove objekata možda će biti potrebno da se objekti ručno kreiraju u usluzi Azure Active Directory.

Ako vam je potrebna dodatna pomoć, otvorite ulaznicu za podršku i navedite opseg problema (uključujući tip objekta u koji šaljete) kako bismo vam lakše pomogli.