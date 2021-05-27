---
title: Zalihe softvera nedostaju ili su netačni
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11382"
- "9001470"
ms.openlocfilehash: e886a53f8c063b5395dd002a7d16186985584d72
ms.sourcegitcommit: 0c104e2bd34ccc09bcea389e470692e92bcf1f8f
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 05/26/2021
ms.locfileid: "52676513"
---
# <a name="software-inventory-is-missing-or-inaccurate"></a><span data-ttu-id="73ae5-102">Zalihe softvera nedostaju ili su netačni</span><span class="sxs-lookup"><span data-stu-id="73ae5-102">Software inventory is missing or inaccurate</span></span>

<span data-ttu-id="73ae5-103">Zalihe softvera u softveru Upravljanje pretnjama i ranjivim mestima (TVM) su lista poznatog softvera u organizaciji sa zvaničnim uobičajenim navodima platforme (CPE).</span><span class="sxs-lookup"><span data-stu-id="73ae5-103">The software inventory in threat and vulnerability management (TVM) is a list of known software in your organization with official Common Platform Enumerations (CPE).</span></span>

<span data-ttu-id="73ae5-104">Softverski proizvodi bez zvaničnog CPE-a nisu objavili ranjivosti.</span><span class="sxs-lookup"><span data-stu-id="73ae5-104">Software products without an official CPE don’t have vulnerabilities published.</span></span> <span data-ttu-id="73ae5-105">Zalihe obuhvataju i detalje kao što su ime prodavca, broj slabosti, pretnje i broj izloženih uređaja.</span><span class="sxs-lookup"><span data-stu-id="73ae5-105">The inventory also includes details such as the name of the vendor, number of weaknesses, threats, and number of exposed devices.</span></span>

<span data-ttu-id="73ae5-106">Promene softvera na uređajima obično se odražavaju na bezbednosnim portalima u roku od dva sata.</span><span class="sxs-lookup"><span data-stu-id="73ae5-106">Software changes on devices are typically reflected in security portals within two hours.</span></span> <span data-ttu-id="73ae5-107">Međutim, ponekad može potrajati duže.</span><span class="sxs-lookup"><span data-stu-id="73ae5-107">However, it may sometimes take longer.</span></span> <span data-ttu-id="73ae5-108">Trenutno ne postoji način da se na silom sinhronizuje; ovo je tekuća neprekidna procena.</span><span class="sxs-lookup"><span data-stu-id="73ae5-108">There’s currently no way to force a sync; this is an ongoing continuous assessment.</span></span>

<span data-ttu-id="73ae5-109">Ako ste napravili promenu softvera i promena se ne odražava ispravno na TVM nakon 5 časova, pratite ove korake:</span><span class="sxs-lookup"><span data-stu-id="73ae5-109">If you made a software change and the change is not accurately reflected in TVM after 5 hours, follow these steps:</span></span>

1. <span data-ttu-id="73ae5-110">Proverite odeljak sa dokazema softvera da biste razumeli kako je softver otkriven.</span><span class="sxs-lookup"><span data-stu-id="73ae5-110">Check the software evidence section to understand how the software was detected.</span></span>
1. <span data-ttu-id="73ae5-111">Uverite se da je softver podržan.</span><span class="sxs-lookup"><span data-stu-id="73ae5-111">Make sure that the software is supported.</span></span> <span data-ttu-id="73ae5-112">Softver može biti vidljiv samo na nivou uređaja čak i ako ga Upravljanje pretnjama i ranjivim mestima.</span><span class="sxs-lookup"><span data-stu-id="73ae5-112">Software may be visible only at the device level even if it is currently not supported by threat and vulnerability management.</span></span> <span data-ttu-id="73ae5-113">Međutim, dostupni su samo ograničeni podaci.</span><span class="sxs-lookup"><span data-stu-id="73ae5-113">However, only limited data is available.</span></span>
1. <span data-ttu-id="73ae5-114">Korake za prijavu netačnosti sa portala možete da vidite u izveštaju ["Neprecizno"](/microsoft-365/security/defender-endpoint/tvm-software-inventory?view=o365-worldwide#report-inaccuracy).</span><span class="sxs-lookup"><span data-stu-id="73ae5-114">For steps to report the inaccuracy from the portal, see [Report inaccuracy](/microsoft-365/security/defender-endpoint/tvm-software-inventory?view=o365-worldwide#report-inaccuracy).</span></span>
   
    <span data-ttu-id="73ae5-115">**Na primer:** Izveštavanje o netačnosti sa MDE portala je jednostupni kanal za inženjering.</span><span class="sxs-lookup"><span data-stu-id="73ae5-115">**Note**: Reporting an inaccuracy from the MDE portal is a one-way channel to engineering.</span></span> <span data-ttu-id="73ae5-116">Ako je problem hitan, otvorite tiket za podršku.</span><span class="sxs-lookup"><span data-stu-id="73ae5-116">If the issue is urgent, open a support ticket.</span></span>

<span data-ttu-id="73ae5-117">Više informacija potražite u temi [Softverski zalihe – Upravljanje pretnjama i ranjivim mestima.](/microsoft-365/security/defender-endpoint/tvm-software-inventory)</span><span class="sxs-lookup"><span data-stu-id="73ae5-117">For more information, see [Software inventory - threat and vulnerability management](/microsoft-365/security/defender-endpoint/tvm-software-inventory).</span></span>