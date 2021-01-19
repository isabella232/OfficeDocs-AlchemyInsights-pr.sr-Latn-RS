---
title: Dozvole za odobravanje
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/18/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004353"
- "7784"
ms.openlocfilehash: 9e686bd33414512b0a3a2bc24477832a508537a8
ms.sourcegitcommit: 7b213fd5e8a3fdb5c602673dc194d576d372ac96
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901614"
---
# <a name="grant-permissions"></a><span data-ttu-id="ce62a-102">Dozvole za odobravanje</span><span class="sxs-lookup"><span data-stu-id="ce62a-102">Grant permissions</span></span>

1. <span data-ttu-id="ce62a-103">**Dodeljivanje administracije za administraciju na nivou zakupca**: pogledajte saglasnost za administratore administracije za dodelu stanara [na prijavu](https://docs.microsoft.com/azure/active-directory/manage-apps/grant-admin-consent) za uputstvo za odobravanje zakupca za pristup zakupcu sa Azure lokacije, pomoću Azure AD PowerShell ili iz samoga odziva.</span><span class="sxs-lookup"><span data-stu-id="ce62a-103">**Granting tenant-wide admin consent**: See [Grant tenant-wide admin consent to an application](https://docs.microsoft.com/azure/active-directory/manage-apps/grant-admin-consent) for step-by-step instructions for granting tenant-wide admin consent from the Azure portal, using Azure AD PowerShell, or from the consent prompt itself.</span></span>
1. <span data-ttu-id="ce62a-104">**Davanje pristanka u ime određenog korisnika**: umesto dodeljivanja pristanka za celu organizaciju, administrator može da koristi i [Microsoft Graph API](https://docs.microsoft.com/graph/use-the-api) za odobravanje saglasnosti za delegirane dozvole u ime jednog korisnika.</span><span class="sxs-lookup"><span data-stu-id="ce62a-104">**Granting consent on behalf of a specific user**: Instead of granting consent for the entire organization, an administrator can also use the [Microsoft Graph API](https://docs.microsoft.com/graph/use-the-api) to grant consent to delegated permissions on behalf of a single user.</span></span> <span data-ttu-id="ce62a-105">Više informacija potražite u članku [pristup pristupu u ime korisnika](https://docs.microsoft.com/graph/auth-v2-user).</span><span class="sxs-lookup"><span data-stu-id="ce62a-105">For more information, see [Get access on behalf of a user](https://docs.microsoft.com/graph/auth-v2-user).</span></span>