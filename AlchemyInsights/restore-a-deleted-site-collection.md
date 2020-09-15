---
title: Vraćanje izbrisane Veb lokacija
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cf7521c3-97b4-465a-97eb-6c0a41338a30
ms.openlocfilehash: 570284765f32212b4ef2062db5b70f427b28c121
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47692057"
---
# <a name="restore-a-deleted-site"></a><span data-ttu-id="1b365-102">Vraćanje izbrisane Veb lokacija</span><span class="sxs-lookup"><span data-stu-id="1b365-102">Restore a deleted site</span></span>

<span data-ttu-id="1b365-103">Kada administrator izbriše SharePoint lokaciju, ona se nalazi u korpi za otpatke kolekcije lokacija, gde se čuva za 93 dana pre nego što se trajno izbriše.</span><span class="sxs-lookup"><span data-stu-id="1b365-103">When an admin deletes a SharePoint site, it's placed in the site collection Recycle Bin, where it's kept for 93 days before it's permanently deleted.</span></span> <span data-ttu-id="1b365-104">Da biste vratili sajt u prethodno stanje:</span><span class="sxs-lookup"><span data-stu-id="1b365-104">To restore the site:</span></span>
  
1. <span data-ttu-id="1b365-105">U novom SharePoint centru administracije izaberite stavku **Korpa za otpatke** na traci.</span><span class="sxs-lookup"><span data-stu-id="1b365-105">In the new SharePoint admin center, click **Recycle Bin** on the ribbon.</span></span> 
    
2. <span data-ttu-id="1b365-106">Potvrdite izbor u polju za potvrdu pored kolekcije lokacija koju želite da vratite u prethodno stanje.</span><span class="sxs-lookup"><span data-stu-id="1b365-106">Select the check box next to the site collection you want to restore.</span></span>
    
3. <span data-ttu-id="1b365-107">Kliknite na dugme **Vrati izbrisane stavke**.</span><span class="sxs-lookup"><span data-stu-id="1b365-107">Click **Restore Deleted Items**.</span></span>
    
<span data-ttu-id="1b365-108">Da biste vratili izbrisane lokacije za komunikaciju, možete da koristite novi SharePoint centar administracije.</span><span class="sxs-lookup"><span data-stu-id="1b365-108">To restore a deleted communication site, you can use the new SharePoint admin center.</span></span> <span data-ttu-id="1b365-109">U suprotnom, treba da koristite Microsoft PowerShell.</span><span class="sxs-lookup"><span data-stu-id="1b365-109">Otherwise, you need to use Microsoft PowerShell.</span></span> <span data-ttu-id="1b365-110">Da biste vratili lokaciju koja pripada Microsoft 365 grupi, morate da vratite grupu u Exchange centar administracije.</span><span class="sxs-lookup"><span data-stu-id="1b365-110">To restore a site that belongs to a Microsoft 365 group, you need to restore the group in the Exchange admin center.</span></span> <span data-ttu-id="1b365-111">Grupe mogu da se obnove 30 dana nakon brisanja.</span><span class="sxs-lookup"><span data-stu-id="1b365-111">Groups can be restored for 30 days after they're deleted.</span></span>
  

