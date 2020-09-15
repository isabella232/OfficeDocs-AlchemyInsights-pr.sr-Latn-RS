---
title: 1332 OWA – pravila prijemnog poštanskog sandučeta se ne primenjuju za poštansko sanduče
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1332"
- "3700002"
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: f4d8db9c590abc490f193ef54a8a1dc5afba82b9
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47721605"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a>Pravilo prijemnog poštanskog sandučeta ne funkcioniše na očekivani način

Potvrdite sledeće postavke u programu Outlook na vebu:

- Poruka može ponovo da se preusmerava, prosledi ili odgovori na automatski osnovu pravila iz prijemnog poštanskog sandučeta. Pravilo preusmeravanja (pravilo prijemnog poštanskog sandučeta ili pravilo toka pošte, takođe poznato kao pravilo transporta) može da doda najviše 10 primalaca prosleđivanja u poruku. Više informacija potražite u članku [ograničenja pravila naloga, transporta i prijemnog poštanskog sandučeta](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).

- Pravila prijemnog poštanskog sandučeta ne funkcionišu na alternativnom poštanskom sandučetu. Više informacija o alternativnom poštanskom sandučetu, potražite u članku [alternativni poštanske poštansko sanduče](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).

Da biste rešili ove probleme, pogledajte [članak KB 2829319](https://support.microsoft.com/kb/2829319).

Ako se prethodni problemi ne primenjuju, ponovo potražite izveštaj o dijagnostici za pravilo prijemnog poštanskog sandučeta pre nego što eskalirate problem na Microsoft podršku:

1. Otvorite poštansko sanduče u programu Outlook na vebu i kliknite na dugme <img src='data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABIAAAASCAMAAABhEH5lAAAA51BMVEX6+fj6+fDr+fjK+fj69LRxsuj6+cjY+fi/+fin3ev6+ddMk81HdK5AaatHLn/ntXTrsW5cRmLOk0pAND5KNCl1NCOi3fiGwvjJ3fDBz+F6teFgpdt6stX68c314syTucirtchum8bjz8BQh7/6+b47fbrKtapiian63aFDaaHJuZJiQo36woVabH7ZtHiOQnTHm2wlKmqriWF/cFzVnVTFjlSyeUkrNEmBLkWfaUGsaT67fTrj9Pi19PjO8fiv5vj69OFWm9Pt3aZ1Qo0lNHQ1P2iYTWGOQmHcpV5kRlqvc0mrbERpPzMoEeekAAAAxElEQVQY03WQ5w6CUAyFy3Jv3HsrICoKqLj3fP/nsTcNakjsn9t+bW/OKfyL6iTCc49e/ktuRs2WEhE1U/qgQQfEzGkNyxzVXLdw0ASW+a7BZp3HpJ+cpovUjcv6PYtvSmKj4/SswTMaBgg9FQF5axWysKoson4cGMYCvlEAQDwK7XkZwEVbRBpDPC46ygbAbPl31p4Wvd8nwiRCLnIArJb1ZBD7KFWMkdQLSUVIhowsGaIwzzVHikfVV8lzHPv3OGTfTd4gnRNqGdZ49AAAAABJRU5ErkJggg==' />
 **Postavke**  >  **Prikaz svih postavki**  >  programa Outlook **Pošte**  >  **Pravila**.

2. Na dnu stranice kliknite na dugme **Ako pravila ne funkcionišu kliknite ovde da biste generisali izveštaj o dijagnostici**.
