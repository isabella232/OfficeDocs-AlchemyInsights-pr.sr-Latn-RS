---
title: Alatka za izvoz e-otkrivanja
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
- "263"
- "928"
- "1100001"
- "3100022"
ms.assetid: b16d310d-1134-4959-be68-d1c0ad463930
ms.openlocfilehash: 67e59182a5053111a08f5fb2be814931a1aa815d
ms.sourcegitcommit: fbe6925797cab0b38172386f1b059dc122e452a4
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/25/2020
ms.locfileid: "48277954"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a><span data-ttu-id="84744-102">Ne možete da instalirate ili pokrećete alatku za izvoz eDiscovery?</span><span class="sxs-lookup"><span data-stu-id="84744-102">Can't install or run the eDiscovery Export Tool?</span></span>

<span data-ttu-id="84744-103">Ako ne možete da instalirate ili izvršite alatku za izvoz eDiscovery za preuzimanje rezultata pretrage, potvrdite sledeće stvari:</span><span class="sxs-lookup"><span data-stu-id="84744-103">If you can't install or run the eDiscovery Export Tool to download search results, check the following things:</span></span>
  
- <span data-ttu-id="84744-104">Računar koji koristite ispunjava ove unapred zahteve:</span><span class="sxs-lookup"><span data-stu-id="84744-104">The computer you're using meets these pre-requisites:</span></span>

  - <span data-ttu-id="84744-105">32-ili 64-bitne verzije operativnog sistema Windows 7 i novije verzije</span><span class="sxs-lookup"><span data-stu-id="84744-105">32- or 64-bit versions of Windows 7 and later versions</span></span>

  - <span data-ttu-id="84744-106">Microsoft .NET Framework 4.7</span><span class="sxs-lookup"><span data-stu-id="84744-106">Microsoft .NET Framework 4.7</span></span>

  - <span data-ttu-id="84744-107">Podržani pregledač:</span><span class="sxs-lookup"><span data-stu-id="84744-107">A supported browser:</span></span>

  - <span data-ttu-id="84744-108">Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="84744-108">Microsoft Edge</span></span>

    <span data-ttu-id="84744-109">Jer</span><span class="sxs-lookup"><span data-stu-id="84744-109">Or</span></span>

  - <span data-ttu-id="84744-110">Internet Explorer 10 i novije verzije</span><span class="sxs-lookup"><span data-stu-id="84744-110">Internet Explorer 10 and later versions</span></span>

    <span data-ttu-id="84744-111">Drugi pregledači, na primer Google Chrome i Mozilla Firefox nisu podržani.</span><span class="sxs-lookup"><span data-stu-id="84744-111">Other browsers, such as Google Chrome and Mozilla Firefox aren't supported.</span></span>

- <span data-ttu-id="84744-112">Vaša organizacija može da se poveže sa krajnjim tačkom u Azure, što je \*\* \* . BLOB.Core.Windows.net\*\* (džoker predstavlja Jedinstveni identifikator za posao izvoza).</span><span class="sxs-lookup"><span data-stu-id="84744-112">Your organization can connect to the endpoint in Azure, which is **\*.blob.core.windows.net** (the wildcard represents a unique identifier for your export job).</span></span>

- <span data-ttu-id="84744-113">Dodeljena vam je uloga izvoza u Microsoft 365 bezbednosnom &amp; centru za usaglašenost.</span><span class="sxs-lookup"><span data-stu-id="84744-113">You're assigned the Export role in the Microsoft 365 Security &amp; Compliance Center.</span></span> <span data-ttu-id="84744-114">Ova uloga se podrazumevano dodeljuje samo grupi uloga programa eDiscovery.</span><span class="sxs-lookup"><span data-stu-id="84744-114">By default, this role is only assigned to the eDiscovery Manager role group.</span></span> <span data-ttu-id="84744-115">Pogledajte [dodelu dozvola za eDiscovery](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions).</span><span class="sxs-lookup"><span data-stu-id="84744-115">See [Assign eDiscovery permissions](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions).</span></span>

<span data-ttu-id="84744-116">Više informacija potražite u članku [izvoz rezultata pretrage sadržaja](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).</span><span class="sxs-lookup"><span data-stu-id="84744-116">For more information, see [Export Content Search results](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).</span></span>

<span data-ttu-id="84744-117">Ako izvozite više od 100K poštanskih sandučića, moraćete da koristite sledeće PowerShell za preuzimanje rezultata izvoza:  [izvoz rezultata iz više od 100k poštanskih sandučića](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).</span><span class="sxs-lookup"><span data-stu-id="84744-117">If you are exporting more than 100K mailboxes, you will need to use the following Powershell to download the Export results:  [Exporting results from more than 100K mailboxes](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).</span></span>