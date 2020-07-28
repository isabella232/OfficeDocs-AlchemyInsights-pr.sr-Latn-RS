---
title: Nije moguće promeniti korisničko ime
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1729"
- "9000183"
ms.openlocfilehash: 34aecdf503699ee500179f0958158fc964d77fcb
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 07/28/2020
ms.locfileid: "45440300"
---
# <a name="unable-to-change-username"></a><span data-ttu-id="3c9a2-102">Nije moguće promeniti korisničko ime</span><span class="sxs-lookup"><span data-stu-id="3c9a2-102">Unable to change UserName</span></span>

<span data-ttu-id="3c9a2-103">U nekim slučajevima, UPN (UserPrincipalName) promene nisu razdeljene u oblaku.</span><span class="sxs-lookup"><span data-stu-id="3c9a2-103">In some cases, UPN (UserPrincipalName) changes aren't propagated to the cloud.</span></span> <span data-ttu-id="3c9a2-104">Možete da primite greške pri proveri valjanosti na Office 365 portalu ili da ne možete da promenite korisničko ime ili e-adresu.</span><span class="sxs-lookup"><span data-stu-id="3c9a2-104">You might receive validation errors in the Office 365 portal or be unable to change the username or email address.</span></span> <span data-ttu-id="3c9a2-105">Da biste rešili ovaj problem, ručno podesite UserPrincipalName koristeći ovu komandu "PowerShell".</span><span class="sxs-lookup"><span data-stu-id="3c9a2-105">To resolve this issue, manually set UserPrincipalName using this PowerShell command.</span></span>

<span data-ttu-id="3c9a2-106">**Primer: preimenovanje korisnika**</span><span class="sxs-lookup"><span data-stu-id="3c9a2-106">**Example: Rename a user**</span></span>

<span data-ttu-id="3c9a2-107">PowerShellCopy</span><span class="sxs-lookup"><span data-stu-id="3c9a2-107">PowerShellCopy</span></span>

<span data-ttu-id="3c9a2-108">PS C: \> Set-MsolUserPrincipalName-Korisnikprincipalname "davidc@contoso.com"-NewUserPrincipalName "davidchew@contoso.com"</span><span class="sxs-lookup"><span data-stu-id="3c9a2-108">PS C:\> Set-MsolUserPrincipalName -UserPrincipalName "davidc@contoso.com" -NewUserPrincipalName "davidchew@contoso.com"</span></span>

<span data-ttu-id="3c9a2-109">Ova komanda preimenuje davidc@contoso.com na davidchew@contoso.com.</span><span class="sxs-lookup"><span data-stu-id="3c9a2-109">This command renames davidc@contoso.com to davidchew@contoso.com.</span></span>

<span data-ttu-id="3c9a2-110">Više informacija potražite u članku [Postavljanje-MsolUserPrincipalName](https://docs.microsoft.com/powershell/module/msonline/set-msoluserprincipalname?view=azureadps-1.0).</span><span class="sxs-lookup"><span data-stu-id="3c9a2-110">For more information, see [Set-MsolUserPrincipalName](https://docs.microsoft.com/powershell/module/msonline/set-msoluserprincipalname?view=azureadps-1.0).</span></span>