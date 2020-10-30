---
title: Promena zahteva jakih lozinki
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
- "9000105"
- "1600"
ms.openlocfilehash: 8ce331275e066b5a4f177ae27178ec726f90762f
ms.sourcegitcommit: aa35d2e1829f7d07f64fb891bf73b1fd80f0864c
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 10/30/2020
ms.locfileid: "48804437"
---
# <a name="change-strong-password-requirement"></a>Promena zahteva jakih lozinki

Microsoft podrazumevano zahteva velike lozinke.

Pomoću programa PowerShell možete da onemogućite velike lozinke za određene korisnike sa ovim komandama:

`Set-MsolUser –UserPrincipalName <UserPrincipalName> –StrongPasswordRequired  $false`

Da biste onemogućili velike lozinke za sve korisnike, koristite:

`Get-MsolUser | Set-MsolUser -StrongPasswordRequired $false`

- [Više informacija o smernicama za lozinke](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [Kako da se povežete sa uslugom Microsoft 365 pomoću programa PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [Više informacija o PowerShell MsolUser komandama](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)
