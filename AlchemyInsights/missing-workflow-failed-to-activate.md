---
title: Tok posla koji nedostaje nije uspeo da se aktivira
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: 604dc770c5c14ded6a8de1cec9e311b03b69f094
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47667100"
---
# <a name="missing-workflow-failed-to-activate"></a><span data-ttu-id="5420e-102">Tok posla koji nedostaje nije uspeo da se aktivira</span><span class="sxs-lookup"><span data-stu-id="5420e-102">Missing Workflow Failed to Activate</span></span>

<span data-ttu-id="5420e-103">U Microsoft SharePoint kolekciji lokacija ne možete da dodate globalni tok posla koji se može ponovo koristiti (kao što je "odobravanje-SharePoint 2010") na listu ili u biblioteku.</span><span class="sxs-lookup"><span data-stu-id="5420e-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="5420e-104">Da biste rešili ovaj problem, slijedite ove korake:</span><span class="sxs-lookup"><span data-stu-id="5420e-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="5420e-105">Otvorite osnovnu Veb lokaciju kolekcije lokacija u sistemu SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="5420e-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="5420e-106">U okviru **objekti portala**izaberite stavku **Tokovi posla**.</span><span class="sxs-lookup"><span data-stu-id="5420e-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="5420e-107">U **novom** odeljku trake **tokova posla** izaberite stavku **tok posla**koji je moguće ponovo koristiti.</span><span class="sxs-lookup"><span data-stu-id="5420e-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="5420e-108">Na obrascu **toka posla** koji je moguće ponovo koristiti unesite ime \* \* *Repair2010* \* \*.</span><span class="sxs-lookup"><span data-stu-id="5420e-108">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*.</span></span> <span data-ttu-id="5420e-109">Za **tip platforme**izaberite stavke **SharePoint 2010 tokovi posla**, a zatim kliknite na dugme **u redu**.</span><span class="sxs-lookup"><span data-stu-id="5420e-109">For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="5420e-110">U odeljku **Čuvanje** trake **toka posla** izaberite stavku **Objavi**.</span><span class="sxs-lookup"><span data-stu-id="5420e-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="5420e-111">U odeljku **Upravljanje** traci **toka posla** izaberite stavku objavi na **globalnom nivou**.</span><span class="sxs-lookup"><span data-stu-id="5420e-111">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**.</span></span> <span data-ttu-id="5420e-112">U dijalogu za potvrdu koji se pojavi izaberite stavku **u redu**.</span><span class="sxs-lookup"><span data-stu-id="5420e-112">In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="5420e-113">U Veb pregledaču pronađite osnovnu Veb lokaciju kolekcije lokacija, a zatim Access **Site Settings** \> **funkcije kolekcije lokacija**za postavke lokacije.</span><span class="sxs-lookup"><span data-stu-id="5420e-113">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**.</span></span> <span data-ttu-id="5420e-114">Zatim, preklopnik funkcije **tokova posla** :</span><span class="sxs-lookup"><span data-stu-id="5420e-114">Then, toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="5420e-115">· Ako je funkcija  *aktivirana*  , kliknite na dugme **Deaktiviraj,** a zatim kliknite na dugme **Aktiviraj**.</span><span class="sxs-lookup"><span data-stu-id="5420e-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="5420e-116">· Ako je funkcija  *deaktivirana*  , kliknite na dugme **Aktiviraj**.</span><span class="sxs-lookup"><span data-stu-id="5420e-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="5420e-117">Više informacija potražite u sledećem [članku](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="5420e-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

