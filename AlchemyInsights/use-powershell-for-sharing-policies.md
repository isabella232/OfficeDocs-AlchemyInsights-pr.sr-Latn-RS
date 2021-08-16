---
title: Koristite PowerShell za smernice za deljenje i relacije u organizaciji
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
- "3800014"
- "898"
ms.openlocfilehash: 48df03b1397b0e924aa878cea3d1cac07ca862c3636c1273d10f4841a03fddcf
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "53998481"
---
# <a name="use-powershell-for-sharing-policies-and-organization-relationships"></a>Koristite PowerShell za smernice za deljenje i relacije u organizaciji


Za relacije u organizaciji pregledajte detaljne informacije o sintaksi i parametrima za: [Get-FederationInformation](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation), [New-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship), [Set-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship)  I  [Remove-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship).

Da biste kreirali smernice za deljenje, upotrebite [New-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy). Da biste [primenili smernice za deljenje na poštansko sanduče ili korisnika](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy#use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes) potrebno je da koristite kombinaciju [Set-Mailbox](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) i [Get-Mailbox](https://docs.microsoft.com/powershell/module/exchange/get-mailbox) uz nove kreirane smernice. Da biste [ izmenili, onemogućili ili uklonili smernice za deljenje](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy) potrebno je da koristite [Set-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) i [Remove-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy).

**Da biste potpuno razumeli ovu temu, pročitajte:**

[Deljenje u usluzi Exchange Online](https://docs.microsoft.com/exchange/sharing/sharing)