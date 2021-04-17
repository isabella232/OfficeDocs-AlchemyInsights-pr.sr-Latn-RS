---
title: Promena zahteva za jaku lozinku
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
- "9000105"
- "1600"
ms.openlocfilehash: cf5cab9a1c2dd4226997d93417dc7104347f8a6e
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/15/2021
ms.locfileid: "51818482"
---
# <a name="change-strong-password-requirement"></a>Promena zahteva jake lozinke

Microsoft podrazumevano zahteva jake lozinke.

Pomoću programa PowerShell možete da onemogućite jake lozinke za određene korisnike sa ovim komandama:

`Set-MsolUser –UserPrincipalName <UserPrincipalName> –StrongPasswordRequired  $false`

Da biste onemogućili jake lozinke za sve korisnike, koristite:

`Get-MsolUser | Set-MsolUser -StrongPasswordRequired $false`

- [Više informacija o smernicama za lozinke](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [Kako da se povežete sa uslugom Microsoft 365 pomoću programa PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [Više informacija o PowerShell MsolUser komandama](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)
