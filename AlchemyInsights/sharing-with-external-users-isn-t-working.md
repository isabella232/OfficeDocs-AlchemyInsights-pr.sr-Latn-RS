---
title: Deljenje sa spoljnim korisnicima ne funkcioniše
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: bd3a6c0d7206801ff76be121c4878b8343cc9886
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47691589"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a><span data-ttu-id="a13db-102">Rešavanje problema deljenja SharePoint sadržaja sa spoljnim korisnicima</span><span class="sxs-lookup"><span data-stu-id="a13db-102">Fix problems sharing SharePoint content with external users</span></span>

<span data-ttu-id="a13db-103">Uverite se da je spoljašnje deljenje uključeno za vašu organizaciju:</span><span class="sxs-lookup"><span data-stu-id="a13db-103">Make sure external sharing is turned on for your organization:</span></span>
  
1. <span data-ttu-id="a13db-104">Idite na [ &amp; stranicu programski dodaci usluge u Microsoft 365 centru administracije](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns)i izaberite stavku **lokacije**.</span><span class="sxs-lookup"><span data-stu-id="a13db-104">Go to the [Services &amp; add-ins page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns), and click **Sites**.</span></span>
    
2. <span data-ttu-id="a13db-105">Proverite da li je postavka uključena u "uključeno".</span><span class="sxs-lookup"><span data-stu-id="a13db-105">Make sure the setting is turned to "On."</span></span> <span data-ttu-id="a13db-106">Ako je izabrana stavka "samo postojeći spoljni korisnici", uverite se da je spoljni korisnik naveden u Microsoft 365 centru administracije.</span><span class="sxs-lookup"><span data-stu-id="a13db-106">If "Only existing external users" is selected, make sure the external user is listed in the Microsoft 365 admin center.</span></span>
    
<span data-ttu-id="a13db-107">Proverite da li je spoljni deljenje uključeno za sajt.</span><span class="sxs-lookup"><span data-stu-id="a13db-107">Make sure external sharing it turned on for the site.</span></span> <span data-ttu-id="a13db-108">Za klasičnu kolekciju lokacija:</span><span class="sxs-lookup"><span data-stu-id="a13db-108">For a classic site collection:</span></span>
  
1. <span data-ttu-id="a13db-109">U novom SharePoint centru administracije, u levom oknu izaberite stavku **lokacije**.</span><span class="sxs-lookup"><span data-stu-id="a13db-109">In the new SharePoint admin center, in the left pane, click **sites**.</span></span>
    
2. <span data-ttu-id="a13db-110">Izaberite lokaciju ili lokacije i na traci kliknite na dugme **Deljenje**.</span><span class="sxs-lookup"><span data-stu-id="a13db-110">Select the site or sites, and on the ribbon, click **Sharing**.</span></span>
    
<span data-ttu-id="a13db-111">Za lokaciju tima koja pripada Microsoft 365 grupi ili na lokaciji za komunikaciju:</span><span class="sxs-lookup"><span data-stu-id="a13db-111">For a team site that belongs to a Microsoft 365 group, or a communication site:</span></span>
  
- <span data-ttu-id="a13db-112">Ovi novi tipovi lokacija imaju istu postavku deljenja kao i postavka za celu organizaciju, osim ako postavka za celu organizaciju ne omogućava deljenje datoteka pomoću veza koje ne zahteva prijavljivanje.</span><span class="sxs-lookup"><span data-stu-id="a13db-112">These new site types have the same sharing setting as your organization-wide setting, unless the organization-wide setting allows sharing files using links that don't require sign-in.</span></span> <span data-ttu-id="a13db-113">U ovom slučaju, lokacije omogućava deljenje sa novim i postojećim spoljnim korisnicima koji se prijave.</span><span class="sxs-lookup"><span data-stu-id="a13db-113">In this case, the sites allow sharing with new and existing external users who sign in.</span></span> <span data-ttu-id="a13db-114">Da biste promenili postavku za određene lokacije, koristite novi SharePoint centar administracije ili PowerShell.</span><span class="sxs-lookup"><span data-stu-id="a13db-114">To change the setting for specific sites, use the new SharePoint admin center or PowerShell.</span></span> <span data-ttu-id="a13db-115">[Saznajte više](https://go.microsoft.com/fwlink/?linkid=871863).</span><span class="sxs-lookup"><span data-stu-id="a13db-115">[Learn more](https://go.microsoft.com/fwlink/?linkid=871863).</span></span>
    
> [!NOTE]
> <span data-ttu-id="a13db-116">Postavke spoljnog deljenja za bilo koju stranicu mogu da budu restriktivnije od vaše postavke za celu organizaciju, ali ne i više od toga.</span><span class="sxs-lookup"><span data-stu-id="a13db-116">The external sharing setting for any site can be more restrictive than your organization-wide setting, but not more permissive than the organization-wide setting.</span></span> 
  

