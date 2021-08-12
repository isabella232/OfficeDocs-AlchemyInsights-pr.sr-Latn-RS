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
ms.openlocfilehash: 4530abb3bf597458ea22441203a0db24b4b109f0760258310072891014c4b454
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "53929319"
---
# <a name="create-a-group"></a>Kreiranje grupe

Ova tema opisuje kreiranje grupa.

**Dozvola za kreiranje grupe**

Uverite se da ste ovlašćeni za kreiranje nove grupe. Globalni administratori mogu da onemoguće kreiranje grupa na Azure portalu ili na Access tabli. Možda će vam biti potreban administrator da biste napravili novu grupu za vas ili da bi vam dao odgovarajuće dozvole.

**Upravljanje dozvolama za kreiranje grupe**

1. Globalni administratori mogu da upravljaju dozvolama za kreiranje grupa (iz bezbednosnih razloga) ili Office 365 grupama kreiranim na Azure portalu ili na tabli za pristup tako što će u opcijama "Korisnici mogu da kreiraju bezbednosne grupe na Azure portalima" ili "Korisnici mogu da kreiraju Office 365 grupe na Azure portalima" u opcijama Sve grupe opšte   >  **(Postavke).**
2. Možete i da ograničite kreiranje grupa da biste izabrali grupu korisnika ako imate licencu Azure Active Directory P1 Premium grupe.

**Zabrana obaveštenja o dobrodošlici za nove Office 365 članove grupe**

Obaveštenje dobrodošlice poslato korisnicima koji su dodati u Office 365 grupe može se onemogućiti postavljanjem **funkcije UnifiedGroupWelcomeMessageEnabled** na False u programu Powershell. Više o ovoj postavki [saznajte ovde.](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true)

