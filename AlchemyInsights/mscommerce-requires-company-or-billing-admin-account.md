---
title: Povezivanje u MSCommerce module
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
- "9001212"
- "3529"
ms.openlocfilehash: 357604f1d4cda3ac8ef6b8b4dbf8780b96dcee59409a6c2edad4a84d6adda62a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "53974683"
---
# <a name="mscommerce-requires-a-company-or-billing-administrator-account"></a>MSCommerce zahteva nalog administratora preduzeća ili naplate

Modul MSCommerce zahteva nalog sa privilegijama administratora preduzeća ili naplate. Ako dobijate sledeću grešku, potrebno je da se ponovo vežete sa drugim nalogom.

*ErrorMessage – Udaljeni server je vratio grešku: (403) Zabranjeno. ErrorDetails - na C:\Program Files\WindowsPowerShell\Modules\MSCommerce\1.2\MSCommerce.psm1:216 char:5*<br>
*+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;HandleError -ErrorContext $_ -CustomErrorMessage "Nije uspelo poništi izbor...*<br>
\+&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*+ CategoryInfo: NotSpecified: (:) [Write-error], WriteErrorException*<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;*+ FullyQualifiedErrorId : Microsoft.PowerShell.Commands.WriteErrorException,HandleError*

Ako vaš nalog nema privilegije preduzeća ili administratora naplate, obratite se IT administratoru.
