---
title: 1332 ova-pravila prijemnog poštanskog sandučeta ne izvršava se za poštansko sanduče
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1332"
- "3700002"
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: 9abdcdcb33d39b8b9fe2df80f0c15a8b55e465fd
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 06/05/2020
ms.locfileid: "44576574"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a>Pravilo prijemnog poštanskog sandučeta ne funkcioniše na očekivani način

Proverite sledeće postavke u programu Outlook na Webu:

- Poruka može da se preusmeravaju, prosleđuje ili da automatski radi na osnovu pravila prijemnog poštanskog sandučeta. Pravilo preusmeravanja (pravilo prijemnog poštanskog sandučeta ili pravila za protok pošte, takođe poznato kao pravilo za prenos) može da doda najviše deset primalaca prosleđivanja poruci. Više informacija potražite u članku [ograničenje pravila za dnevnik, saobraćaj i prijemno poštansko sanduče](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).

- Pravila prijemnog poštanskog sandučeta ne funkcionišu na alternativnoj evidentiranje poštanskom sandučetu. Za više informacija o alternativnoj evidentiranje poštanskom sandučetu pogledajte [alternativni evidentiranje poštansko sanduče](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).

Da biste rešili ove probleme, pogledajte [KB 2829319](https://support.microsoft.com/kb/2829319).

Ako se prethodni problemi ne primenjuju, pokrenite dijagnostički izveštaj pravila prijemnog poštanskog sandučeta pre nego što se problem proširi na Microsoft podršku:

1. Otvorite poštansko sanduče u programu Outlook na vebu i kliknite na dugme <img src='data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABIAAAASCAMAAABhEH5lAAAA51BMVEX6+fj6+fDr+fjK+fj69LRxsuj6+cjY+fi/+fin3ev6+ddMk81HdK5AaatHLn/ntXTrsW5cRmLOk0pAND5KNCl1NCOi3fiGwvjJ3fDBz+F6teFgpdt6stX68c314syTucirtchum8bjz8BQh7/6+b47fbrKtapiian63aFDaaHJuZJiQo36woVabH7ZtHiOQnTHm2wlKmqriWF/cFzVnVTFjlSyeUkrNEmBLkWfaUGsaT67fTrj9Pi19PjO8fiv5vj69OFWm9Pt3aZ1Qo0lNHQ1P2iYTWGOQmHcpV5kRlqvc0mrbERpPzMoEeekAAAAxElEQVQY03WQ5w6CUAyFy3Jv3HsrICoKqLj3fP/nsTcNakjsn9t+bW/OKfyL6iTCc49e/ktuRs2WEhE1U/qgQQfEzGkNyxzVXLdw0ASW+a7BZp3HpJ+cpovUjcv6PYtvSmKj4/SswTMaBgg9FQF5axWysKoson4cGMYCvlEAQDwK7XkZwEVbRBpDPC46ygbAbPl31p4Wvd8nwiRCLnIArJb1ZBD7KFWMkdQLSUVIhowsGaIwzzVHikfVV8lzHPv3OGTfTd4gnRNqGdZ49AAAAABJRU5ErkJggg==' />
 **Postavke**  >  **Prikaz svih postavki**  >  programa Outlook **Pošte**  >  **Pravila**.

2. Na dnu stranice kliknite **Ako vaša pravila ne rade kliknite ovde da biste generisali dijagnostički izveštaj**.
