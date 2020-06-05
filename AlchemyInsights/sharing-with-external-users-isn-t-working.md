---
title: Deljenje sa spoljnim korisnicima ne radi
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: 9a40f52637bc8aa7894754118f0f862aa6c71fe2
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 06/05/2020
ms.locfileid: "44582789"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a><span data-ttu-id="25179-102">Rešavanje problema sa deljenjem SharePoint sadržaja sa spoljnim korisnicima</span><span class="sxs-lookup"><span data-stu-id="25179-102">Fix problems sharing SharePoint content with external users</span></span>

<span data-ttu-id="25179-103">Proverite da li je uključeno zajedničko deljenje za vašu organizaciju:</span><span class="sxs-lookup"><span data-stu-id="25179-103">Make sure external sharing is turned on for your organization:</span></span>
  
1. <span data-ttu-id="25179-104">Idite na [stranicu " &amp; programski dodaci za usluge" u Microsoft 365 admin Center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns)i izaberite stavku **lokacije**.</span><span class="sxs-lookup"><span data-stu-id="25179-104">Go to the [Services &amp; add-ins page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), and click **Sites**.</span></span>
    
2. <span data-ttu-id="25179-105">Proverite da li je postavka uključena u "uključeno".</span><span class="sxs-lookup"><span data-stu-id="25179-105">Make sure the setting is turned to "On."</span></span> <span data-ttu-id="25179-106">Ako je izabrano "samo postojeći spoljni korisnici", uverite se da je spoljni korisnik naveden u Microsoft 365 admin Center.</span><span class="sxs-lookup"><span data-stu-id="25179-106">If "Only existing external users" is selected, make sure the external user is listed in the Microsoft 365 admin center.</span></span>
    
<span data-ttu-id="25179-107">Uverite se da je spoljna podela uključena za lokaciju.</span><span class="sxs-lookup"><span data-stu-id="25179-107">Make sure external sharing it turned on for the site.</span></span> <span data-ttu-id="25179-108">Za klasičnu kolekciju lokacija:</span><span class="sxs-lookup"><span data-stu-id="25179-108">For a classic site collection:</span></span>
  
1. <span data-ttu-id="25179-109">U novom SharePoint administratoru centra, u levom oknu izaberite stavku **lokacije**.</span><span class="sxs-lookup"><span data-stu-id="25179-109">In the new SharePoint admin center, in the left pane, click **sites**.</span></span>
    
2. <span data-ttu-id="25179-110">Izaberite lokaciju ili lokacije i na glavnoj traci kliknite na dugme **Deljenje**.</span><span class="sxs-lookup"><span data-stu-id="25179-110">Select the site or sites, and on the ribbon, click **Sharing**.</span></span>
    
<span data-ttu-id="25179-111">Za lokaciju tima koja pripada Microsoft 365 grupi ili lokaciji za komunikaciju:</span><span class="sxs-lookup"><span data-stu-id="25179-111">For a team site that belongs to a Microsoft 365 group, or a communication site:</span></span>
  
- <span data-ttu-id="25179-112">Ovi novi tipovi lokacija imaju istu postavku deljenja kao i postavke za celu organizaciju, osim ako postavka za celu organizaciju ne dozvoljava deljenje datoteka pomoću veza koje ne zahtevaju prijavljivanje.</span><span class="sxs-lookup"><span data-stu-id="25179-112">These new site types have the same sharing setting as your organization-wide setting, unless the organization-wide setting allows sharing files using links that don't require sign-in.</span></span> <span data-ttu-id="25179-113">U ovom slučaju, lokacije omogućavaju deljenje sa novim i postojećim spoljnim korisnicima koji se prijave.</span><span class="sxs-lookup"><span data-stu-id="25179-113">In this case, the sites allow sharing with new and existing external users who sign in.</span></span> <span data-ttu-id="25179-114">Da biste promenili postavke za određene lokacije, koristite novi SharePoint admin Center ili PowerShell.</span><span class="sxs-lookup"><span data-stu-id="25179-114">To change the setting for specific sites, use the new SharePoint admin center or PowerShell.</span></span> <span data-ttu-id="25179-115">[Saznajte više](https://go.microsoft.com/fwlink/?linkid=871863).</span><span class="sxs-lookup"><span data-stu-id="25179-115">[Learn more](https://go.microsoft.com/fwlink/?linkid=871863).</span></span>
    
> [!NOTE]
> <span data-ttu-id="25179-116">Postavka spoljnog deljenja za svaku lokaciju može da bude restriktivnija od postavke za celu organizaciju, ali ne i veća od postavke za celu organizaciju.</span><span class="sxs-lookup"><span data-stu-id="25179-116">The external sharing setting for any site can be more restrictive than your organization-wide setting, but not more permissive than the organization-wide setting.</span></span> 
  

