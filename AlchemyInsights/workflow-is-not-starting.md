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
ms.openlocfilehash: e3b8777ed74b812b31338784999eea43a95d3456
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/15/2020
ms.locfileid: "47794781"
---
# <a name="workflow-is-not-starting"></a><span data-ttu-id="ac748-102">Tok posla se ne pokreće</span><span class="sxs-lookup"><span data-stu-id="ac748-102">Workflow is not starting</span></span>

- <span data-ttu-id="ac748-103">SharePoint 2010 i SharePoint 2013 tokovi posla ne počinju.</span><span class="sxs-lookup"><span data-stu-id="ac748-103">SharePoint 2010 and SharePoint 2013 workflows are not starting.</span></span>

    - <span data-ttu-id="ac748-104">Ako se tok posla ne pokreće, možda postoji privremeni problem pri uslugama gde korisnici mogu da doživljaju prekida kašnjenja sa napretkom toka posla.</span><span class="sxs-lookup"><span data-stu-id="ac748-104">If your workflow is not starting, there may be a temporary service issue where users may experience intermittent delays with workflow progress.</span></span> <span data-ttu-id="ac748-105">Pogledajte [kontrolnu tablu zdrave usluge](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) da biste videli da li je vaša organizacija uticala na njih.</span><span class="sxs-lookup"><span data-stu-id="ac748-105">Check the [Service Health Dashboard](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>

    - <span data-ttu-id="ac748-106">Ako je prošlo više od 24 časa od kada ste prvi put videli ovaj problem, prijavite karticu podrške.</span><span class="sxs-lookup"><span data-stu-id="ac748-106">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="ac748-107">U mnogim slučajevima, već radimo na rešenju.</span><span class="sxs-lookup"><span data-stu-id="ac748-107">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="ac748-108">Dajte nam najmanje 24 časa da biste dovršili rešenje.</span><span class="sxs-lookup"><span data-stu-id="ac748-108">Please give us at least 24 hours to complete a solution.</span></span>

- <span data-ttu-id="ac748-109">SharePoint 2010 tokovi posla odloženi na početnom meniju.</span><span class="sxs-lookup"><span data-stu-id="ac748-109">SharePoint 2010 workflows delayed on start.</span></span>

    - <span data-ttu-id="ac748-110">Do ovoga dolazi ako je tok posla izazvan velikim grupama.</span><span class="sxs-lookup"><span data-stu-id="ac748-110">This occurs if the workflow is triggered in large batches.</span></span> <span data-ttu-id="ac748-111">(na primer, kada se odjednom doda nekoliko stavki).</span><span class="sxs-lookup"><span data-stu-id="ac748-111">(for example, when several items are added at once).</span></span>

    - <span data-ttu-id="ac748-112">Tokovi posla nisu dizajnirani za pokretanje u realnom vremenu, tako da je kašnjenje po dizajnu dizajn.</span><span class="sxs-lookup"><span data-stu-id="ac748-112">Workflows are not designed to run real-time, so a delay is by-design behavior.</span></span>

   -  <span data-ttu-id="ac748-113">Ako je tok posla složen Extensible Object Markup Language (XMOL), kompilacija može biti spora.</span><span class="sxs-lookup"><span data-stu-id="ac748-113">If the Workflow is complex Extensible Object Markup Language (XMOL), compilation can be slow.</span></span> <span data-ttu-id="ac748-114">Potvrdite [ovaj](https://support.microsoft.com//kb/3043697) članak.</span><span class="sxs-lookup"><span data-stu-id="ac748-114">Check [this](https://support.microsoft.com//kb/3043697) article.</span></span>

    - <span data-ttu-id="ac748-115">Trebalo bi da pojednostavite tok posla ili da ga ponovo dizajnirate pomoću programa Microsoft SharePoint 2013 toka posla.</span><span class="sxs-lookup"><span data-stu-id="ac748-115">You should simplify the workflow or redesign it using the Microsoft SharePoint 2013 Workflow platform type.</span></span>

    - <span data-ttu-id="ac748-116">Ako je vaša istorija toka posla porasla, možda ćete želeti da očistite stavke ili da kreirate novu listu istorije.</span><span class="sxs-lookup"><span data-stu-id="ac748-116">If your workflow history has grown large, you may want to purge the items or create a new history list.</span></span>

        <span data-ttu-id="ac748-117">Više informacija: [Čišćenje istorije toka posla](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span><span class="sxs-lookup"><span data-stu-id="ac748-117">More Information : [Purge Workflow History](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span></span>


## <a name="related-topics"></a><span data-ttu-id="ac748-118">Сродне теме</span><span class="sxs-lookup"><span data-stu-id="ac748-118">Related topics</span></span>
<span data-ttu-id="ac748-119">Želite da probate Microsoft flow u usluzi SharePoint online?</span><span class="sxs-lookup"><span data-stu-id="ac748-119">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="ac748-120">Kreiranje protoka</span><span class="sxs-lookup"><span data-stu-id="ac748-120">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="ac748-121">SharePoint i protok</span><span class="sxs-lookup"><span data-stu-id="ac748-121">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


