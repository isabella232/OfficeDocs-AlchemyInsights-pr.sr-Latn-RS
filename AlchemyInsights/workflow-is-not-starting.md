---
title: Tok posla se ne pokreće
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: e69f3e529e4a2202f641cb62f42b1a20d774a398
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/29/2021
ms.locfileid: "51403757"
---
# <a name="workflow-is-not-starting"></a><span data-ttu-id="3ddeb-102">Tok posla se ne pokreće</span><span class="sxs-lookup"><span data-stu-id="3ddeb-102">Workflow is not starting</span></span>

- <span data-ttu-id="3ddeb-103">SharePoint 2010 i SharePoint 2013 tokovi posla se ne počinju.</span><span class="sxs-lookup"><span data-stu-id="3ddeb-103">SharePoint 2010 and SharePoint 2013 workflows are not starting.</span></span>

    - <span data-ttu-id="3ddeb-104">Ako se tok posla ne pokreće, možda postoji privremeni problem sa uslugom gde korisnici mogu imati povremena odlaganja sa tokom toka posla.</span><span class="sxs-lookup"><span data-stu-id="3ddeb-104">If your workflow is not starting, there may be a temporary service issue where users may experience intermittent delays with workflow progress.</span></span> <span data-ttu-id="3ddeb-105">Proverite [kontrolnu tablu za zdravlje usluge](https://admin.microsoft.com/AdminPortal/Home/servicehealth) da biste videli da li ima uticaja na vašu organizaciju.</span><span class="sxs-lookup"><span data-stu-id="3ddeb-105">Check the [Service Health Dashboard](https://admin.microsoft.com/AdminPortal/Home/servicehealth) to see if your organization is impacted.</span></span>

    - <span data-ttu-id="3ddeb-106">Ako je prošlo više od 24 časa od kada ste prvi put videli ovaj problem, prijavite tiket za podršku.</span><span class="sxs-lookup"><span data-stu-id="3ddeb-106">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="3ddeb-107">U mnogim slučajevima već radimo na rešenju.</span><span class="sxs-lookup"><span data-stu-id="3ddeb-107">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="3ddeb-108">Dajte nam najmanje 24 sata da dovršimo rešenje.</span><span class="sxs-lookup"><span data-stu-id="3ddeb-108">Please give us at least 24 hours to complete a solution.</span></span>

- <span data-ttu-id="3ddeb-109">SharePoint 2010 tokovi posla odloženi pri pokretanju.</span><span class="sxs-lookup"><span data-stu-id="3ddeb-109">SharePoint 2010 workflows delayed on start.</span></span>

    - <span data-ttu-id="3ddeb-110">To se dešava ako se tok posla pokrene u velikim grupama.</span><span class="sxs-lookup"><span data-stu-id="3ddeb-110">This occurs if the workflow is triggered in large batches.</span></span> <span data-ttu-id="3ddeb-111">(Na primer, kada se istovremeno doda nekoliko stavki).</span><span class="sxs-lookup"><span data-stu-id="3ddeb-111">(for example, when several items are added at once).</span></span>

    - <span data-ttu-id="3ddeb-112">Tokovi posla nisu dizajnirani za pokretanje u realnom vremenu, pa je odlaganje ponašanje po dizajnu.</span><span class="sxs-lookup"><span data-stu-id="3ddeb-112">Workflows are not designed to run real-time, so a delay is by-design behavior.</span></span>

   -  <span data-ttu-id="3ddeb-113">Ako je tok posla složen jezik za naznake extensible Object Markup (XMOL), kompajlacija može biti spora.</span><span class="sxs-lookup"><span data-stu-id="3ddeb-113">If the Workflow is complex Extensible Object Markup Language (XMOL), compilation can be slow.</span></span> <span data-ttu-id="3ddeb-114">Pogledajte [ovaj](https://support.microsoft.com//kb/3043697) članak.</span><span class="sxs-lookup"><span data-stu-id="3ddeb-114">Check [this](https://support.microsoft.com//kb/3043697) article.</span></span>

    - <span data-ttu-id="3ddeb-115">Trebalo bi da pojednostaviti tok posla ili ga redizajnovati pomoću tipa platforme Microsoft SharePoint 2013 toka posla.</span><span class="sxs-lookup"><span data-stu-id="3ddeb-115">You should simplify the workflow or redesign it using the Microsoft SharePoint 2013 Workflow platform type.</span></span>

    - <span data-ttu-id="3ddeb-116">Ako je vaša istorija toka posla velika, možda ćete želeti da ih iščistite ili da napravite novu listu istorije.</span><span class="sxs-lookup"><span data-stu-id="3ddeb-116">If your workflow history has grown large, you may want to purge the items or create a new history list.</span></span>

        <span data-ttu-id="3ddeb-117">Više informacija: [Purge Workflow History](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span><span class="sxs-lookup"><span data-stu-id="3ddeb-117">More Information : [Purge Workflow History](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span></span>


## <a name="related-topics"></a><span data-ttu-id="3ddeb-118">Сродне теме</span><span class="sxs-lookup"><span data-stu-id="3ddeb-118">Related topics</span></span>
<span data-ttu-id="3ddeb-119">Želite da isprobate Microsoft Flow u sistemu SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="3ddeb-119">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="3ddeb-120">Kreiranje toka</span><span class="sxs-lookup"><span data-stu-id="3ddeb-120">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="3ddeb-121">SharePoint i Flow</span><span class="sxs-lookup"><span data-stu-id="3ddeb-121">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 
