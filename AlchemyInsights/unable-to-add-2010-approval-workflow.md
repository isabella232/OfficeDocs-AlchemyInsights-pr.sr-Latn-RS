---
title: Nije moguće dodati 2010 tok posla za odobravanje
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 0df65cf9-7eae-4de7-88e9-1914635c8d11
ms.openlocfilehash: aa61f1615b60d27cffad15f02f6ce5dbac1b607f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47699749"
---
# <a name="unable-to-add-2010-approval-workflow"></a><span data-ttu-id="84be5-102">Nije moguće dodati 2010 tok posla za odobravanje</span><span class="sxs-lookup"><span data-stu-id="84be5-102">Unable to add 2010 Approval Workflow</span></span>

<span data-ttu-id="84be5-103">U Microsoft SharePoint kolekciji lokacija ne možete da dodate globalni tok posla koji se može ponovo koristiti (kao što je "odobravanje-SharePoint 2010") na listu ili u biblioteku.</span><span class="sxs-lookup"><span data-stu-id="84be5-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="84be5-104">Da biste rešili ovaj problem, slijedite ove korake:</span><span class="sxs-lookup"><span data-stu-id="84be5-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="84be5-105">Otvorite osnovnu Veb lokaciju kolekcije lokacija u sistemu SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="84be5-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="84be5-106">U okviru **objekti portala**izaberite stavku **Tokovi posla**.</span><span class="sxs-lookup"><span data-stu-id="84be5-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="84be5-107">U **novom** odeljku trake **tokova posla** izaberite stavku **tok posla**koji je moguće ponovo koristiti.</span><span class="sxs-lookup"><span data-stu-id="84be5-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="84be5-108">Na obrascu **toka posla** koji je moguće ponovo koristiti unesite ime \* \* *Repair2010* \* \*.</span><span class="sxs-lookup"><span data-stu-id="84be5-108">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*.</span></span> <span data-ttu-id="84be5-109">Za **tip platforme**izaberite stavke **SharePoint 2010 tokovi posla**, a zatim kliknite na dugme **u redu**.</span><span class="sxs-lookup"><span data-stu-id="84be5-109">For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="84be5-110">U odeljku **Čuvanje** trake **toka posla** izaberite stavku **Objavi**.</span><span class="sxs-lookup"><span data-stu-id="84be5-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="84be5-111">U odeljku **Upravljanje** traci **toka posla** izaberite stavku objavi na **globalnom nivou**.</span><span class="sxs-lookup"><span data-stu-id="84be5-111">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**.</span></span> <span data-ttu-id="84be5-112">U dijalogu za potvrdu koji se pojavi izaberite stavku **u redu**.</span><span class="sxs-lookup"><span data-stu-id="84be5-112">In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="84be5-113">U Veb pregledaču pronađite osnovnu Veb lokaciju kolekcije lokacija, a zatim Access **Site Settings** \> **funkcije kolekcije lokacija**za postavke lokacije.</span><span class="sxs-lookup"><span data-stu-id="84be5-113">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**.</span></span> <span data-ttu-id="84be5-114">Preklopnik funkcije **tokova posla** :</span><span class="sxs-lookup"><span data-stu-id="84be5-114">Toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="84be5-115">· Ako je funkcija  *aktivirana*  , kliknite na dugme **Deaktiviraj,** a zatim kliknite na dugme **Aktiviraj**.</span><span class="sxs-lookup"><span data-stu-id="84be5-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="84be5-116">· Ako je funkcija  *deaktivirana*  , kliknite na dugme **Aktiviraj**.</span><span class="sxs-lookup"><span data-stu-id="84be5-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="84be5-117">Više informacija potražite u sledećem [članku](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="84be5-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

