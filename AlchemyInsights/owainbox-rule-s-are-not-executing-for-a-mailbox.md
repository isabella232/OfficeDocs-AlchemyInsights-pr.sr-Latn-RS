---
title: 1332 OWA – Pravila prijemnog poštanskog sandučeta se ne izvršavaju za poštansko sanduče
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
ms.openlocfilehash: b05ed9f0ee8c18b49b5338c53e67a79f1bf65464385dfa0ebd0639172a1b18f2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "54040916"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a>Pravilo prijemnog poštanskog sandučeta ne funkcioniše na očekivani način

Proverite sledeće postavke u programu Outlook na vebu:

- Poruka može biti automatski preusmerena, prosleđena ili odgovorila na automatski na osnovu pravila prijemnog poštanskog sandučeta samo jednom. Pravilo preusmeravanja (pravilo za prijemno poštansko sanduče ili pravilo protoka pošte, poznato i kao pravilo za prenos) može da doda najviše deset primalaca prosleđivanja poruci. Više informacija potražite u temi [Dnevnik, Prenos i Ograničenja pravila prijemnog poštanskog sandučeta.](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits)

- Pravila prijemnog poštanskog sandučeta ne rade na alternativnom poštanskom sandučetu dnevnika. Dodatne informacije o alternativnom poštanskom sandučetu za dnevnik potražite u temi [Alternativno poštansko sanduče dnevnika](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).

Da biste rešili ove probleme, pogledajte [2829319 KB.](https://support.microsoft.com/kb/2829319)

Ako se prethodni problemi ne primenjuju, pokrenite dijagnostički izveštaj pravila prijemnog poštanskog sandučeta pre nego što problem preskočite microsoft podršci:

1. Otvorite poštansko sanduče u programu Outlook na vebu i kliknite na dugme <img src='data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABIAAAASCAMAAABhEH5lAAAA51BMVEX6+fj6+fDr+fjK+fj69LRxsuj6+cjY+fi/+fin3ev6+ddMk81HdK5AaatHLn/ntXTrsW5cRmLOk0pAND5KNCl1NCOi3fiGwvjJ3fDBz+F6teFgpdt6stX68c314syTucirtchum8bjz8BQh7/6+b47fbrKtapiian63aFDaaHJuZJiQo36woVabH7ZtHiOQnTHm2wlKmqriWF/cFzVnVTFjlSyeUkrNEmBLkWfaUGsaT67fTrj9Pi19PjO8fiv5vj69OFWm9Pt3aZ1Qo0lNHQ1P2iYTWGOQmHcpV5kRlqvc0mrbERpPzMoEeekAAAAxElEQVQY03WQ5w6CUAyFy3Jv3HsrICoKqLj3fP/nsTcNakjsn9t+bW/OKfyL6iTCc49e/ktuRs2WEhE1U/qgQQfEzGkNyxzVXLdw0ASW+a7BZp3HpJ+cpovUjcv6PYtvSmKj4/SswTMaBgg9FQF5axWysKoson4cGMYCvlEAQDwK7XkZwEVbRBpDPC46ygbAbPl31p4Wvd8nwiRCLnIArJb1ZBD7KFWMkdQLSUVIhowsGaIwzzVHikfVV8lzHPv3OGTfTd4gnRNqGdZ49AAAAABJRU5ErkJggg==' />
 **Postavke**  >  **Prikaži sve Outlook Postavke**  >  **Pošta**  >  **Pravila**.

2. Na dnu stranice izaberite stavku Ako pravila ne rade kliknite ovde da biste generisli **dijagnostički izveštaj.**
