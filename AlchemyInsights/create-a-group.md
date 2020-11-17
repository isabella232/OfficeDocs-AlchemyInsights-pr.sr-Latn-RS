---
title: Kreiranje grupe
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
- "9003234"
- "7230"
ms.openlocfilehash: b8cb3f1de991bfe7197607d5e8964a018e31c122
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 11/17/2020
ms.locfileid: "49089174"
---
# <a name="create-a-group"></a>Kreiranje grupe

Ova tema opisuje Kreiranje grupe.

**Dozvola za kreiranje grupe**

Uverite se da ste ovlašćeni za kreiranje nove grupe. Globalni administratori mogu da onemoguće Kreiranje grupe na Azure portovu ili Access tabli. Možda će vam biti potreban administrator da biste kreirali novu grupu za vas ili da biste vam dali odgovarajuće dozvole.

**Upravljanje dozvolama za kreiranje grupe**

1. Globalni administratori mogu da upravljaju dozvolama za kreiranje grupe (iz bezbednosnih razloga) ili Office 365 grupama kreirane na Azure portovi ili Access tabli, tako što ćete izabrati "korisnici mogu da kreiraju bezbednosne grupe u Azure portali" ili "korisnici mogu da kreiraju Office 365 grupe u Azure portali" **All groups**  >  **(postavke)**.
2. Možete i da ograničite Kreiranje grupe da biste izabrali grupu korisnika ako imate licencu za Azure Active Directory P1 Premium.

**Onemogućavanje obaveštenja o dobrodošlici za nove Office 365 članove grupe**

Obaveštenje o dobrodošlici koje se šalju korisnicima koji se dodaju u Office 365 grupe mogu da se onemogućavaju postavljanjem **sindikalnog polja omogućeno** u PowerShell. Saznajte više o ovoj podešavanju [ovde](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).

