---
title: Rešavanje problema sa proverom identiteta toka
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: c15fed9f-65c6-422e-9d32-87e889a44b51
ms.openlocfilehash: 3c4ad806ed446803d8c1e0ba17b3a06d591985d9
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47690581"
---
# <a name="troubleshoot-flow-authentication-errors"></a><span data-ttu-id="ee9af-102">Rešavanje problema sa proverom identiteta toka</span><span class="sxs-lookup"><span data-stu-id="ee9af-102">Troubleshoot Flow authentication errors</span></span>

<span data-ttu-id="ee9af-103">U mnogim slučajevima protok ne radi zbog greške potvrde identiteta.</span><span class="sxs-lookup"><span data-stu-id="ee9af-103">In many cases, flows fail because of an authentication error.</span></span> <span data-ttu-id="ee9af-104">Ako imate ovaj tip greške, poruka o grešci sadrži "neovlašćeno" ili kôd greške 401 ili 403.</span><span class="sxs-lookup"><span data-stu-id="ee9af-104">If you have this type of error, the error message contains "Unauthorized," or an error code of 401 or 403 appears.</span></span> <span data-ttu-id="ee9af-105">Možete da popravite grešku potvrde identiteta tako što ćete ažurirati vezu:</span><span class="sxs-lookup"><span data-stu-id="ee9af-105">You can usually fix an authentication error by updating the connection:</span></span>
  
1. <span data-ttu-id="ee9af-106">Na vrhu veb portala kliknite ili dodirnite ikonu zupčanika da biste otvorili meni postavke, a zatim izaberite ili dodirnite stavku **veze**.</span><span class="sxs-lookup"><span data-stu-id="ee9af-106">At the top of the web portal, click or tap the gear icon to open the Settings menu, and then click or tap **Connections**.</span></span>
    
2. <span data-ttu-id="ee9af-107">Pomerajte se do veze za koju ste videli neovlašćenu poruku o grešci.</span><span class="sxs-lookup"><span data-stu-id="ee9af-107">Scroll to the connection for which you saw the Unauthorized error message.</span></span>
    
3. <span data-ttu-id="ee9af-108">Pored veze, kliknite ili dodirnite vezu **verifikovanja lozinke** u poruci o grešci koja nije autentični.</span><span class="sxs-lookup"><span data-stu-id="ee9af-108">Next to the connection, click or tap the **Verify password** link in the message about the connection not being authenticated.</span></span> 
    
4. <span data-ttu-id="ee9af-109">Verifikujte akreditive tako što ćete slediti uputstva koja se pojavljuju, vratite se na otkazivanje protoka, a zatim kliknite na dugme **ponovo prosledi**.</span><span class="sxs-lookup"><span data-stu-id="ee9af-109">Verify your credentials by following the instructions that appear, return to your flow-run failure, and then click or tap **Resubmit**.</span></span>
    
<span data-ttu-id="ee9af-110">Dodatne pomoći potražite u članku [Rešavanje problema sa protokom](https://go.microsoft.com/fwlink/?linkid=872110).</span><span class="sxs-lookup"><span data-stu-id="ee9af-110">For more help, see [Troubleshooting a flow](https://go.microsoft.com/fwlink/?linkid=872110).</span></span>
  

