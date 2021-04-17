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
ms.openlocfilehash: 7800a447c5dfcc8397121e1149921916ff7944ac
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819094"
---
# <a name="change-email-address-of-a-microsoft-365-group-or-microsoft-teams"></a>Promena e-adrese Microsoft 365 Group ili e-adrese aplikacije Microsoft Teams

Možete da promenite e-adresu grupe Microsoft 365 Group ili e-adresu aplikacije Microsoft Teams [Microsoft 365 centar administracije](https://admin.microsoft.com/). Samo izaberite grupu i izaberite stavku @uredi e-adresu.

Možete da koristite i sledeće EXO PowerShell komande da biste promenili primarnu SMTP adresu Microsoft 365 grupe/aplikacije Teams:

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

Primer:

`Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`
