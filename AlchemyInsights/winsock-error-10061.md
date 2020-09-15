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
ms.openlocfilehash: 4f8007bd8ccb4666260c75fdca15dd0b14eb4e96
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47698876"
---
# <a name="winsock-error-10061"></a>Winsock greška 10061

Ovaj kôd greške znači da Microsoft nije mogao da uspostavi TCP priključak (vezu) sa ciljem ciljnog domaćina. Najverovatniji uzrok ove greške je problem sa konfiguracijom zaštitnog zida. Da biste rešili problem, potvrdite izbor u ovim postavkama:

- Verifikacija konfiguracije zaštitnog zida pomoću informacija u [Microsoft 365 URL adresama i opsezima IP adresa](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

- Ako je greška karakteristična za Exchange online Protection (EOP), trebalo je da budete prethodno obavešteni na [IP adrese Exchange online Protection](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).

- Potvrdite da dobavljač Internet usluga (ISP) ne blokira port.

- Potvrdite pametne postavke domaćina i odredišne servere u konektorima.

Imajte na umu da Microsoft 365 ne blokira *dolazne* veze na ovaj način.
