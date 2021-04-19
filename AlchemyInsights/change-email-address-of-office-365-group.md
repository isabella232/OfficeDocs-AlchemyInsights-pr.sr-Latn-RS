---
title: Promena adrese e-pošte Microsoft 365 grupe
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
ms.openlocfilehash: 8eaafae8650a8072cdfbec281afe6d5e93fea655
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819058"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a>Promena adrese e-pošte Microsoft 365 grupe

Možete da promenite adresu e-pošte Microsoft 365 grupe pomoću centra za administaciju. Samo izaberite grupu i izaberite stavku @uredi e-adresu.

Možete da koristite i komandu EXO PowerShell da biste promenili primarnu SMTP adresu Microsoft 365 grupe:

Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>

Primer:

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
