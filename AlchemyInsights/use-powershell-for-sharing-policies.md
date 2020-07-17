---
title: Korišćenje PowerShell za deljenje smernica i odnosa sa organizacijom
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3800014"
- "898"
ms.openlocfilehash: 717cdd6827e243ac6bf375209a911937c97088d2
ms.sourcegitcommit: 722e9a0ed058cb1eab2dd053be2418b60f7d4aac
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 06/23/2020
ms.locfileid: "44862154"
---
# <a name="use-powershell-for-sharing-policies-and-organization-relationships"></a><span data-ttu-id="aee43-102">Korišćenje PowerShell za deljenje smernica i odnosa sa organizacijom</span><span class="sxs-lookup"><span data-stu-id="aee43-102">Use PowerShell for Sharing policies and Organization relationships</span></span>


<span data-ttu-id="aee43-103">Za relacije između organizacija Pregledajte detaljnu sintaksu i informacije o parametrima za: [Preuzimanje informacija](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation), [novo-organizationarelaciju](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship), [skup-organizationrelacija](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship) i [Uklanjanje-organizationrelacija](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship).</span><span class="sxs-lookup"><span data-stu-id="aee43-103">For Organization relationships please review the detailed syntax and parameter information for : [Get-FederationInformation](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation), [New-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship), [Set-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship)  AND  [Remove-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship).</span></span>

<span data-ttu-id="aee43-104">Da biste kreirali smernice za deljenje koristite [novu smernicu](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy).</span><span class="sxs-lookup"><span data-stu-id="aee43-104">To create sharing policy use [New-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy).</span></span> <span data-ttu-id="aee43-105">Da biste [primenili smernice za deljenje na poštansko sanduče ili korisnika](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy%23use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes) , potrebno je da koristite kombinaciju [Set-poštansko sanduče](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) i [poštanskog sandučeta](https://docs.microsoft.com/powershell/module/exchange/get-mailbox) sa Novokreiranim smernicama.</span><span class="sxs-lookup"><span data-stu-id="aee43-105">To  [apply a sharing policy to a mailbox or user](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy%23use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes)  you need to use a combination of  [Set-Mailbox](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) and [Get-Mailbox](https://docs.microsoft.com/powershell/module/exchange/get-mailbox) with the newly created policy.</span></span> <span data-ttu-id="aee43-106">Da biste [izmenili, onemogućili ili uklonili smernice za deljenje](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy) koje su vam potrebne da biste koristili smernice za [Podešavanje](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) i [Uklanjanje](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy)smernica.</span><span class="sxs-lookup"><span data-stu-id="aee43-106">To  [modify, disable or remove a sharing policy](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy)  you need to use  [Set-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) and [Remove-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy).</span></span>

<span data-ttu-id="aee43-107">**Za potpuno razumevanje ove teme molimo vas da pročitate:**</span><span class="sxs-lookup"><span data-stu-id="aee43-107">**For full understanding of this topic please read:**</span></span>

[<span data-ttu-id="aee43-108">Deljenje u programu Exchange online</span><span class="sxs-lookup"><span data-stu-id="aee43-108">Sharing in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/sharing)