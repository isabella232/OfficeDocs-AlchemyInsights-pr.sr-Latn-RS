---
title: Nije vraćen nijedan rezultat tokom pretrage/izvoza sadržaja
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3200003"
- "7463"
ms.openlocfilehash: db025cd1278471a3c54d55409d9a9418095778a7
ms.sourcegitcommit: 9c64886a9e1a9b0ff356b28a5c1482ecc148d7ef
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 12/14/2020
ms.locfileid: "49680326"
---
# <a name="no-results-returned-during-content-searchexport"></a><span data-ttu-id="92972-102">Nije vraćen nijedan rezultat tokom pretrage/izvoza sadržaja</span><span class="sxs-lookup"><span data-stu-id="92972-102">No results returned during Content Search/Export</span></span>

<span data-ttu-id="92972-103">Ako imate problema sa sledećim scenarijima za eDiscovery:</span><span class="sxs-lookup"><span data-stu-id="92972-103">If you are experiencing issues with the following eDiscovery scenarios:</span></span>

- <span data-ttu-id="92972-104">Pretraga sadržaja/izvoz ne vraća podatke ili neočekivane podatke</span><span class="sxs-lookup"><span data-stu-id="92972-104">Content Search/Export returns no data or unexpected data</span></span>
- <span data-ttu-id="92972-105">Pretraga e-otkrivanja ili izvoz nije uspeo</span><span class="sxs-lookup"><span data-stu-id="92972-105">eDiscovery Search or Export fails</span></span>

<span data-ttu-id="92972-106">To može biti izazvano određenim bezbednosnim filteri usaglašenosti koje je postavio određeni administrator i koji nisu komunicirali sa svim administratorima.</span><span class="sxs-lookup"><span data-stu-id="92972-106">This may be caused due to certain Compliance Security Filters that were setup by a specific Admin and not been communicated to all Admins.</span></span>

<span data-ttu-id="92972-107">Da biste rešili ovaj problem, uverite se da postoje filteri za bezbednost usaglašenosti koji možda uzrokuju ove probleme:</span><span class="sxs-lookup"><span data-stu-id="92972-107">To resolve this, check if there are any Compliance Security Filters that may be causing these issues:</span></span>

1. <span data-ttu-id="92972-108">Povezivanje sa PowerShell centra za bezbednost i usaglašenost</span><span class="sxs-lookup"><span data-stu-id="92972-108">Connect to Security and Compliance Center Powershell</span></span>
2. <span data-ttu-id="92972-109">Uradite sledeće zapovesti:</span><span class="sxs-lookup"><span data-stu-id="92972-109">Run the following commandlets:</span></span>

    `$org = “yourdomain.com”`

    `Get-ComplianceSecurityFilter -Organization $org`

<span data-ttu-id="92972-110">Dodatne informacije o bezbednosnim filterima usaglašenosti potražite [u članku filtriranje dozvola za pretraživanje sadržaja](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)</span><span class="sxs-lookup"><span data-stu-id="92972-110">For additional information on Compliance Security Filters, see [Permissions Filtering for Content Search](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)</span></span>
