---
title: Promena e-adrese Microsoft 365 Group ili e-adrese aplikacije Microsoft Teams
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
ms.openlocfilehash: acb343553bfb7e100c03d0e7046ed5cbdd6b739b9a61e3faf17768bd8aadff34
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "53995636"
---
# <a name="change-email-address-of-a-microsoft-365-group-or-microsoft-teams"></a>Promena e-adrese Microsoft 365 Group ili e-adrese aplikacije Microsoft Teams

Možete da promenite e-adresu grupe Microsoft 365 Group ili e-adresu aplikacije Microsoft Teams [Microsoft 365 centar administracije](https://admin.microsoft.com/). Samo izaberite grupu i izaberite stavku @uredi e-adresu.

Možete da koristite i sledeće EXO PowerShell komande da biste promenili primarnu SMTP adresu Microsoft 365 grupe/aplikacije Teams:

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

Primer:

`Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`
