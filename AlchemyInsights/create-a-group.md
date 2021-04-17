---
title: Kreiranje grupe
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
- "9003234"
- "7230"
ms.openlocfilehash: ec74b7c098d302d3bdeb5a412fad41efe7b82b98
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816375"
---
# <a name="create-a-group"></a>Kreiranje grupe

Ova tema opisuje kreiranje grupa.

**Dozvola za kreiranje grupe**

Uverite se da ste ovlašćeni za kreiranje nove grupe. Globalni administratori mogu da onemoguće kreiranje grupa na Azure portalu ili na Access tabli. Možda će vam biti potreban administrator da biste napravili novu grupu za vas ili da bi vam dao odgovarajuće dozvole.

**Upravljanje dozvolama za kreiranje grupe**

1. Globalni administratori mogu da upravljaju dozvolama za kreiranje grupa (iz bezbednosnih razloga) ili Office 365 grupama kreiranim na Azure portalu ili na tabli za pristup, tako što će u opcijama "Korisnici mogu da kreiraju bezbednosne grupe na Azure portalima" ili "Korisnici mogu da kreiraju Office 365 grupe na Azure portalima" u opcijama Sve grupe Opšte  >  **(Postavke).**
2. Možete i da ograničite kreiranje grupa da biste izabrali grupu korisnika ako imate Azure Active Directory P1 Premium licencu.

**Kako da neometano obaveštenje o dobrodošlici za nove članove Office 365 grupe**

Obaveštenje dobrodošlice poslato korisnicima koji su dodati u Office 365 grupe može se onemogućiti postavljanjem **funkcije UnifiedGroupWelcomeMessageEnabled** na False u programu PowerShell. Više o ovoj postavki [saznajte ovde.](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true)

