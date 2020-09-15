---
title: Pretraga sadržaja nema rezultata
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
- "9000661"
- "2527"
ms.openlocfilehash: 1e90c403556a317ff810971ccfa4a91694fb1171
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47680661"
---
# <a name="no-results-from-content-searchexports"></a><span data-ttu-id="dd505-102">Nema rezultata pretrage sadržaja/izvoza</span><span class="sxs-lookup"><span data-stu-id="dd505-102">No results from Content Search/Exports</span></span>

<span data-ttu-id="dd505-103">Problemi sa pretraživanjem sadržaja/izvozom koji se ne vraća, mogu da budu uzrok određenog bezbednosnog proizvoda koji je podesio određeni administrator i da se ne javlja svim administratorima.</span><span class="sxs-lookup"><span data-stu-id="dd505-103">Issues with Content Search/Exports not returning any data may be due to certain Compliance Security Filter that was setup by a specific Admin and not communicating it to all Admins.</span></span>

<span data-ttu-id="dd505-104">Da biste rešili ovo, pogledajte da li postoje filteri za bezbednost usaglašenosti koji možda uzrokuju sledeće:</span><span class="sxs-lookup"><span data-stu-id="dd505-104">To resolve this, check to see if there are any Compliance Security Filters that may be causing this:</span></span>
1. <span data-ttu-id="dd505-105">Povezivanje sa PowerShell centra za bezbednost i usaglašenost</span><span class="sxs-lookup"><span data-stu-id="dd505-105">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="dd505-106">Uradite sledeće zapovesti:</span><span class="sxs-lookup"><span data-stu-id="dd505-106">Run the following commandlets:</span></span>
<br><span data-ttu-id="dd505-107">$org = "yourdomain.com"</span><span class="sxs-lookup"><span data-stu-id="dd505-107">$org = “yourdomain.com”</span></span>
<br><span data-ttu-id="dd505-108">Filter za $org</span><span class="sxs-lookup"><span data-stu-id="dd505-108">Get-ComplianceSecurityFilter -Organization $org</span></span>