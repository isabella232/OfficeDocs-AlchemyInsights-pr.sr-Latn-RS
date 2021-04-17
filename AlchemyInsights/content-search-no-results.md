---
title: Nema rezultata pretrage sadržaja
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
- "9000661"
- "2527"
ms.openlocfilehash: 0267286ca5967ee891e65343d49adf776f0322a6
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816862"
---
# <a name="no-results-from-content-searchexports"></a><span data-ttu-id="4ad1b-102">Nema rezultata pretrage/izvoza sadržaja</span><span class="sxs-lookup"><span data-stu-id="4ad1b-102">No results from Content Search/Exports</span></span>

<span data-ttu-id="4ad1b-103">Problemi sa pretragom sadržaja/izvozima koji ne vraćaju podatke mogu da budu zbog određenog filtera za bezbednost usaglašenosti koji je podstagao određeni administator i što ga nije preneo svim dobavljačima.</span><span class="sxs-lookup"><span data-stu-id="4ad1b-103">Issues with Content Search/Exports not returning any data may be due to certain Compliance Security Filter that was setup by a specific Admin and not communicating it to all Admins.</span></span>

<span data-ttu-id="4ad1b-104">Da biste rešili ovo, proverite da li postoje filteri za bezbednost usaglašenosti koji možda uzrokuju ovo:</span><span class="sxs-lookup"><span data-stu-id="4ad1b-104">To resolve this, check to see if there are any Compliance Security Filters that may be causing this:</span></span>
1. <span data-ttu-id="4ad1b-105">Povezivanje sa powershell centrom za bezbednost i usaglašenost</span><span class="sxs-lookup"><span data-stu-id="4ad1b-105">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="4ad1b-106">Pokrenite sledeće komande:</span><span class="sxs-lookup"><span data-stu-id="4ad1b-106">Run the following commandlets:</span></span>
<br><span data-ttu-id="4ad1b-107">$org = "yourdomain.com"</span><span class="sxs-lookup"><span data-stu-id="4ad1b-107">$org = “yourdomain.com”</span></span>
<br><span data-ttu-id="4ad1b-108">Get-ComplianceSecurityFilter -Organization $org</span><span class="sxs-lookup"><span data-stu-id="4ad1b-108">Get-ComplianceSecurityFilter -Organization $org</span></span>