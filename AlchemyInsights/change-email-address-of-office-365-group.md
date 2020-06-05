---
title: Promena e-adrese Microsoft 365 grupe
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "4704"
ms.openlocfilehash: 32968f085a4e9d49f60ef88e4e78bf6c67629556
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: HT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580671"
---
# <a name="change-email-address-of-a-microsoft-365-group"></a>Promena e-adrese Microsoft 365 grupe

E-adresu Microsoft 365 grupe možete da promenite pomoću administratorskog centra. Samo izaberite grupu i izaberite @edit e-adresu.

Takođe možete koristiti sledeću komandu "EXO PowerShell" da biste promenili primarnu SMTP adresu Microsoft 365 grupe:

Set-UnifiedGroup <Group Name> -PrimarySmtpAddress<new SMTP Address>

Primer:

```
    Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com
```
