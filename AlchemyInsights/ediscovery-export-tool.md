---
title: Alatka za izvoz e-discovery
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
- "263"
- "928"
- "1100001"
- "3100022"
ms.assetid: b16d310d-1134-4959-be68-d1c0ad463930
ms.openlocfilehash: b1100175c75fb77a499e706380305eb016cf1b2b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814602"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a><span data-ttu-id="d0ce3-102">Ne možete da instalirate ili pokrenete alatku za izvoz e-discovery?</span><span class="sxs-lookup"><span data-stu-id="d0ce3-102">Can't install or run the eDiscovery Export Tool?</span></span>

<span data-ttu-id="d0ce3-103">Ako ne možete da instalirate ili pokrenete alatku za izvoz e-discovery da biste preuzeli rezultate pretrage, proverite sledeće:</span><span class="sxs-lookup"><span data-stu-id="d0ce3-103">If you can't install or run the eDiscovery Export Tool to download search results, check the following things:</span></span>
  
- <span data-ttu-id="d0ce3-104">Računar koji koristite ispunjava ove preduslove:</span><span class="sxs-lookup"><span data-stu-id="d0ce3-104">The computer you're using meets these pre-requisites:</span></span>

  - <span data-ttu-id="d0ce3-105">32-bitna ili 64-bitna verzija operativnog sistema Windows 7 i novije verzije</span><span class="sxs-lookup"><span data-stu-id="d0ce3-105">32- or 64-bit versions of Windows 7 and later versions</span></span>

  - <span data-ttu-id="d0ce3-106">Microsoft .NET Framework 4.7</span><span class="sxs-lookup"><span data-stu-id="d0ce3-106">Microsoft .NET Framework 4.7</span></span>

  - <span data-ttu-id="d0ce3-107">Podržani pregledač:</span><span class="sxs-lookup"><span data-stu-id="d0ce3-107">A supported browser:</span></span>

  - <span data-ttu-id="d0ce3-108">Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="d0ce3-108">Microsoft Edge</span></span>

    <span data-ttu-id="d0ce3-109">Ili</span><span class="sxs-lookup"><span data-stu-id="d0ce3-109">Or</span></span>

  - <span data-ttu-id="d0ce3-110">Internet Explorer 10 i novije verzije</span><span class="sxs-lookup"><span data-stu-id="d0ce3-110">Internet Explorer 10 and later versions</span></span>

    <span data-ttu-id="d0ce3-111">Drugi pregledači, kao što su Google Chrome i Mozilla Firefox nisu podržani.</span><span class="sxs-lookup"><span data-stu-id="d0ce3-111">Other browsers, such as Google Chrome and Mozilla Firefox aren't supported.</span></span>

- <span data-ttu-id="d0ce3-112">Vaša organizacija može da se poveže sa krajnjim tačkom u programu Azure, što je **\* .blob.core.windows.net** (džoker predstavlja jedinstveni identifikator vašeg posla izvoza).</span><span class="sxs-lookup"><span data-stu-id="d0ce3-112">Your organization can connect to the endpoint in Azure, which is **\*.blob.core.windows.net** (the wildcard represents a unique identifier for your export job).</span></span>

- <span data-ttu-id="d0ce3-113">Dodeljena vam je uloga za izvoz u Microsoft 365 centru za &amp; usaglašenost.</span><span class="sxs-lookup"><span data-stu-id="d0ce3-113">You're assigned the Export role in the Microsoft 365 Security &amp; Compliance Center.</span></span> <span data-ttu-id="d0ce3-114">Ova uloga se podrazumevano dodeljuje samo grupi uloga menadžera e-discovery.</span><span class="sxs-lookup"><span data-stu-id="d0ce3-114">By default, this role is only assigned to the eDiscovery Manager role group.</span></span> <span data-ttu-id="d0ce3-115">Pogledajte [dodela dozvola za e-discovery](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions).</span><span class="sxs-lookup"><span data-stu-id="d0ce3-115">See [Assign eDiscovery permissions](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions).</span></span>

<span data-ttu-id="d0ce3-116">Dodatne informacije potražite u [temi Izvoz rezultata pretrage sadržaja.](https://docs.microsoft.com/microsoft-365/compliance/export-search-results)</span><span class="sxs-lookup"><span data-stu-id="d0ce3-116">For more information, see [Export Content Search results](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).</span></span>

<span data-ttu-id="d0ce3-117">Ako izvozite više od 100K poštannih sandučića, biće potrebno da koristite sledeći PowerShell da biste preuzeli rezultate izvoza: Izvoz rezultata iz više od  [100K](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes)poštannih sandučića.</span><span class="sxs-lookup"><span data-stu-id="d0ce3-117">If you are exporting more than 100K mailboxes, you will need to use the following Powershell to download the Export results:  [Exporting results from more than 100K mailboxes](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).</span></span>