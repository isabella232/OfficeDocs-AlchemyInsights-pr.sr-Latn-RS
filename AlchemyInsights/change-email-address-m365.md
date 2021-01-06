---
title: Promena e-adrese Microsoft 365 Group ili e-adrese aplikacije Microsoft Teams
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "4704"
ms.openlocfilehash: ff7abaf3d8e0ed977eba5712bdd19185738fa75c
ms.sourcegitcommit: 8be59778b7d39213a27a471802eae7fc006eb1ff
ms.translationtype: HT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 01/05/2021
ms.locfileid: "49756571"
---
# <a name="change-email-address-of-a-microsoft-365-group-or-microsoft-teams"></a>Promena e-adrese Microsoft 365 Group ili e-adrese aplikacije Microsoft Teams

Možete da promenite e-adresu grupe Microsoft 365 Group ili e-adresu aplikacije Microsoft Teams [Microsoft 365 centar administracije](https://admin.microsoft.com/). Samo izaberite grupu i izaberite stavku @uredi e-adresu.

Možete da koristite i sledeće EXO PowerShell komande da biste promenili primarnu SMTP adresu Microsoft 365 grupe/aplikacije Teams:

`Set-UnifiedGroup <Group Name> -PrimarySmtpAddress <new SMTP Address>`

Primer:

`Set-UnifiedGroup Marketing -PrimarySmtpAddress marketing@contoso.com`
