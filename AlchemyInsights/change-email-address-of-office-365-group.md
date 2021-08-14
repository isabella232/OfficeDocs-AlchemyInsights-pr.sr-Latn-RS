---
title: Promena e-adrese Microsoft 365 grupe
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "4704"
ms.openlocfilehash: 6bd9301b983d09f6a0058fee17577b9fc695458ed205f96aacf79a87e4a91e34
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "53930743"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a>Promena e-adrese Microsoft 365 grupe

Možete da promenite e-adresu Microsoft 365 grupe pomoću centra za administaciju. Samo izaberite grupu i izaberite stavku @uredi e-adresu.

Možete da koristite i posle EXO PowerShell komande da biste promenili primarnu SMTP adresu Microsoft 365 grupe:

Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>

Primer:

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
