---
title: 1554 Winsock greška 10061
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
- "1554"
- "9000079"
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: 7991f83a0b4791eaa7eb3246f7e61f781e4c7430931fbf920d7fd9e44c018d13
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "54083244"
---
# <a name="winsock-error-10061"></a>Winsock greška 10061

Ovaj kôd greške znači da Microsoft ne može da uspostavi TCP socket (vezu) sa ciljnim hostom. Najverovatnije uzrok ove greške je problem sa konfiguracijom zaštitnog zida. Da biste rešili problem, proverite ove postavke:

- Verifikacija konfiguracije zaštitnog zida sa [informacijama iz Microsoft 365 UL-ovima i IP adresama](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

- Ako je greška specifična za Exchange Online Protection (EOP), trebalo bi da ste prethodno bili obavešteni o promeni [Exchange Online Protection IP adresa.](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)

- Proverite da dobavljač internet usluga (ISP) ne blokira port.

- Proverite postavke pametnog hosta i ciljnog servera u konektorima.

Imajte na Microsoft 365 na ovaj način *ne* blokira dolazne veze.
