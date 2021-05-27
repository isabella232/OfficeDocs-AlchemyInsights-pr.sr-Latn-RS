---
title: Rešavanje problema sa rešavanjem problema čuva greške
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/20/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11274"
- "3200003"
ms.openlocfilehash: 1df2b7153cac99419adc4f72b1c3732e7c746eac
ms.sourcegitcommit: 730efbac8eec016b2b4f83f1b0e01e077f28c444
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 05/20/2021
ms.locfileid: "52676281"
---
# <a name="troubleshooting-ediscovery-holds-errors"></a><span data-ttu-id="953ca-102">Rešavanje problema sa rešavanjem problema čuva greške</span><span class="sxs-lookup"><span data-stu-id="953ca-102">Troubleshooting ediscovery holds errors</span></span>

<span data-ttu-id="953ca-103">Imate problema sa zadržavanjem e-discovery?</span><span class="sxs-lookup"><span data-stu-id="953ca-103">Experiencing issues with eDiscovery holds?</span></span> <span data-ttu-id="953ca-104">Evo nekih najboljih praksi koje treba da razmotrite:</span><span class="sxs-lookup"><span data-stu-id="953ca-104">Here are some best practices to consider:</span></span>

- <span data-ttu-id="953ca-105">Proverite status distribucije zadrške.</span><span class="sxs-lookup"><span data-stu-id="953ca-105">Check the hold distribution status.</span></span>  <span data-ttu-id="953ca-106">Ako je status On **(na čekanju)** ili **Isključeno (na čekanju),** sačekajte da se distribucija zadrške dovrši.</span><span class="sxs-lookup"><span data-stu-id="953ca-106">If status is **On (Pending)** or **Off (Pending)**, wait for hold distribution to complete.</span></span>
- <span data-ttu-id="953ca-107">Objedinite e-discovery držite ispravke u jednom masovnom zahtevu umesto da više puta ažurirate smernice za svaku transakciju.</span><span class="sxs-lookup"><span data-stu-id="953ca-107">Merge eDiscovery hold updates into a single bulk request instead of updating the policy repeatedly for each transaction.</span></span>
- <span data-ttu-id="953ca-108">Pokrenite Set-CaseHoldPolicy <policyname> -RetryDistribution u PowerShell centru za bezbednost i usaglašenost.</span><span class="sxs-lookup"><span data-stu-id="953ca-108">Run Set-CaseHoldPolicy <policyname> -RetryDistribution in the Security and Compliance Center Powershell.</span></span> <span data-ttu-id="953ca-109">Više detalja možete [da Povezivanje u Centar za & usaglašenost za PowerShell.](/powershell/exchange/connect-to-scc-powershell)</span><span class="sxs-lookup"><span data-stu-id="953ca-109">For details, see [Connect to Security & Compliance Center PowerShell](/powershell/exchange/connect-to-scc-powershell).</span></span>

<span data-ttu-id="953ca-110">Korake za proveru ovih postavki i dodatnih najboljih praksi za ublažavanje i [](/microsoft-365/compliance/hold-distribution-errors)rešavanje problema sa čuvanjem e-discovery pogledajte u odeljku Rešavanje problema sa čuvanjem e-otklanjanja.</span><span class="sxs-lookup"><span data-stu-id="953ca-110">For steps to check these settings and additional best practices for mitigating and resolving eDiscovery holds issues, see [Troubleshoot eDiscovery hold errors](/microsoft-365/compliance/hold-distribution-errors).</span></span>
<span data-ttu-id="953ca-111">Informacije o rešavanju drugih uobičajenih problema sa e-disciklanjem potražite u članku Istraživanje, rešavanje uobičajenih problema [sa e-disciklanjem i rešavanje problema sa e-distribucijom.](/microsoft-365/compliance/ediscovery-troubleshooting-common-issues)</span><span class="sxs-lookup"><span data-stu-id="953ca-111">For info about troubleshooting other common eDiscovery issues, see [Investigate, troubleshoot, and resolve common eDiscovery issues](/microsoft-365/compliance/ediscovery-troubleshooting-common-issues).</span></span>
