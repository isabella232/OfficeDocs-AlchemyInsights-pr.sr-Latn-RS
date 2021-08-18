---
title: Outbound relay pool
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/08/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "12315"
ms.openlocfilehash: 7e5bb1fda1dec0c0f72d1944d54b6f2747a6e909
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/13/2021
ms.locfileid: "58326091"
---
# <a name="outbound-relay-pool"></a>Outbound relay pool

Microsoft pravi neke promene u konfiguraciji za slanje ili prosleđivanje e-pošte putem Microsoft 365. Poruke se u određenim scenarijima prosleuju ili se šalju putem Microsoft 365 uz pomoć specijalne relejskog prostore. Poruke poslate korišćenjem relejskog grupa mogu da završe u fascikli sa neželjenom poštom primaoca. Više informacija potražite u temi o [odlaznom isporuki](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages#relay-pool)

Da biste izbegli scenario pomoću grupa releja, uverite se da prosleđene/prenete poruke ispunjavaju jedan od sledećih kriterijuma:

- Odlazni pošiljalac je prihvaćeni domen zakuca.
- SpF) prelazi kada poruka bude u Microsoft 365.
- Pošta koju je identifikovao DomainKeys (DKIM) na domenu pošiljaoca P2 prolaze kada poruka dođe do Microsoft 365.
 
Poruke koje ispunjavaju gorenavedeni kriterijum ne šalju se putem grupa releja.

Ako je MX zapis za domen upućivan na nezavisni ili lokalni server, koristite poboljšano filtriranje da biste se uverili da je SPF provera valjanosti ispravna za dolaznu e-poštu i da biste izbegli slanje e-pošte putem baze podataka.

**Kako da znamo da li to utiče na nas u prostoru releja?**

Ako prosleđene ili prenete e-poruke koriste neki od gorenavedenih kriterijuma, poruke se neće preneti putem grupa releja. Međutim, ako se poruka pošalje putem grupe releja, IP adresu odlaznog servera je u opsegu 40.95.0.0/16, a ime odlaznog servera uključuje **rly** u imenu.

