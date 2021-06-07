---
title: Problemi sa performansama za Microsoft zaštitnik za krajnju tačku na Linux
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11491"
- "9001464"
ms.openlocfilehash: 268f44640d3b2d8764133560d0cbf500eb4afd22
ms.sourcegitcommit: 8242a824491f64be48dfe81da09766920fbd7feb
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 06/06/2021
ms.locfileid: "52794227"
---
# <a name="performance-issues-for-microsoft-defender-for-endpoint-on-linux"></a><span data-ttu-id="74a04-102">Problemi sa performansama za Microsoft zaštitnik za krajnju tačku na Linux</span><span class="sxs-lookup"><span data-stu-id="74a04-102">Performance issues for Microsoft Defender for Endpoint on Linux</span></span>

<span data-ttu-id="74a04-103">Ovaj članak vas vodi kroz korake za identifikovanje problema sa performansama za Microsoft zaštitnik za krajnju tačku na linux-u.</span><span class="sxs-lookup"><span data-stu-id="74a04-103">This article guides you through the steps of identifying performance issues for Microsoft Defender for Endpoint on Linux.</span></span>

<span data-ttu-id="74a04-104">Važno je prvo da proverite da li je problem koji imate rešen u najnovijoj [verziji.](/microsoft-365/security/defender-endpoint/linux-whatsnew)</span><span class="sxs-lookup"><span data-stu-id="74a04-104">It's important to first verify that the problem you're experiencing is resolved with the [latest version](/microsoft-365/security/defender-endpoint/linux-whatsnew).</span></span> 

<span data-ttu-id="74a04-105">Da biste započeli istraživanje, pogledajte [članak Rešavanje problema sa performansama za Microsoft zaštitnik za krajnju tačku na Linux.](/microsoft-365/security/defender-endpoint/linux-support-perf)</span><span class="sxs-lookup"><span data-stu-id="74a04-105">To start your investigation, see [Troubleshoot performance issues for Microsoft Defender for Endpoint on Linux](/microsoft-365/security/defender-endpoint/linux-support-perf).</span></span>

## <a name="exclusions"></a><span data-ttu-id="74a04-106">Izusci</span><span class="sxs-lookup"><span data-stu-id="74a04-106">Exclusions</span></span>

<span data-ttu-id="74a04-107">Izusvi mogu da vam pomognu da ublažite probleme sa performansama.</span><span class="sxs-lookup"><span data-stu-id="74a04-107">Exclusions can help to mitigate performance issues.</span></span> <span data-ttu-id="74a04-108">Pregledajte izuzetke pre nego što počnete kako bi dodatni rizik bio poznat i dokumentovan.</span><span class="sxs-lookup"><span data-stu-id="74a04-108">Review your exclusions before you begin so any additional risk is known and documented.</span></span>

<span data-ttu-id="74a04-109">Više informacija potražite u članku Konfigurisanje izuzetka i provera valjanosti izuzetka za Microsoft zaštitnik za [krajnju tačku na linux-u.](/microsoft-365/security/defender-endpoint/linux-exclusions)</span><span class="sxs-lookup"><span data-stu-id="74a04-109">For more information, see [Configure and validate exclusions for Microsoft Defender for Endpoint on Linux](/microsoft-365/security/defender-endpoint/linux-exclusions).</span></span>

<span data-ttu-id="74a04-110">Kada imate više datoteka koje & izuzmu, a sve se na istoj planini, možda je lakše isključiti planinu.</span><span class="sxs-lookup"><span data-stu-id="74a04-110">When you have multiple files & folders to exclude and they're all on the same mountpoint, it might be easier to exclude the mountpoint.</span></span> <span data-ttu-id="74a04-111">Počev od februarskog izdanja 101.22.80, možete da isključite celu tačku planine.</span><span class="sxs-lookup"><span data-stu-id="74a04-111">Starting with February release 101.22.80, you can exclude an entire mountpoint.</span></span>

<span data-ttu-id="74a04-112">Na primer, ako je /mnt/backup tačka planine, možete da dodate /mnt/backup na listu izuzetih stavki tako što ćete pokrenuti ovu komandu:</span><span class="sxs-lookup"><span data-stu-id="74a04-112">For example, if /mnt/backup is a mountpoint, you can add /mnt/backup to the exclude list by running this command:</span></span>

`$ mdatp exclusion folder add –path /mnt/backup`

<span data-ttu-id="74a04-113">**Napomi:** Dodavanje izuzetka povećava rizik od toga da malver nije otkriven i da ga treba sprovesti i primeniti sa brigom.</span><span class="sxs-lookup"><span data-stu-id="74a04-113">**Note**: Adding exclusions increases the risk of malware not being detected and should be handled and implemented with care.</span></span>

## <a name="need-help"></a><span data-ttu-id="74a04-114">Potrebna vam je pomoć?</span><span class="sxs-lookup"><span data-stu-id="74a04-114">Need Help?</span></span>

<span data-ttu-id="74a04-115">Da biste pomogli na najefikasniji način, prikupite dijagnostične podatke pre nego što otvorite predmet za podršku.</span><span class="sxs-lookup"><span data-stu-id="74a04-115">To assist you in the most efficient way, collect the diagnostic data before opening a support case.</span></span>
