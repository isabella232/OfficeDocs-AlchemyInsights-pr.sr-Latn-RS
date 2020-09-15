---
title: Dodavanje spoljnih korisnika u grupu za distribuciju
ms.author: chrisda
author: chrisda
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: 03cfd2c576cb03cbefd524a4ab6f04e2ef1eebec
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663527"
---
# <a name="add-external-users-to-a-distribution-group"></a><span data-ttu-id="e7deb-102">Dodavanje spoljnih korisnika u grupu za distribuciju</span><span class="sxs-lookup"><span data-stu-id="e7deb-102">Add external users to a Distribution Group</span></span>

<span data-ttu-id="e7deb-103">Dodavanje spoljnog kontakta u grupu za distribuciju (DG) je proces sa dva koraka:</span><span class="sxs-lookup"><span data-stu-id="e7deb-103">Adding an external contact to a Distribution Group (DG) is a two-step process:</span></span>
  
1. <span data-ttu-id="e7deb-104">Kreirajte kontakt e-pošte za spoljnog korisnika:</span><span class="sxs-lookup"><span data-stu-id="e7deb-104">Create a Mail Contact for the external user:</span></span>
    
    1. <span data-ttu-id="e7deb-105">U centru administracije idite na stranicu **Korisnici**  >  [Kontakti](https://admin.microsoft.com/adminportal/home#/Contact) .</span><span class="sxs-lookup"><span data-stu-id="e7deb-105">In the admin center, go to the **Users** > [Contacts](https://admin.microsoft.com/adminportal/home#/Contact) page.</span></span> 
    
    2. <span data-ttu-id="e7deb-106">Izaberite stavku **Dodaj kontakt**.</span><span class="sxs-lookup"><span data-stu-id="e7deb-106">Select **Add a contact**.</span></span>
    
    3. <span data-ttu-id="e7deb-107">Otkucajte informacije za kontakt i izaberite stavku **Dodaj**.</span><span class="sxs-lookup"><span data-stu-id="e7deb-107">Type the information for your contact and select **Add**.</span></span>
    
2. <span data-ttu-id="e7deb-108">Dodajte kontakt e-pošte u svoj DG:</span><span class="sxs-lookup"><span data-stu-id="e7deb-108">Add the Mail Contact to your DG:</span></span>
    
    1. <span data-ttu-id="e7deb-109">U centru administracije idite na stranicu grupe **grupa**  >  [Groups](https://admin.microsoft.com/adminportal/home#/groups) .</span><span class="sxs-lookup"><span data-stu-id="e7deb-109">In the admin center, go to the **Groups** > [Groups](https://admin.microsoft.com/adminportal/home#/groups) page.</span></span> 
    
    2. <span data-ttu-id="e7deb-110">Pronađite generalnog direktora kom želite da dodate spoljnog korisnika i izaberite ga da biste otvorili dijalog uređivanje.</span><span class="sxs-lookup"><span data-stu-id="e7deb-110">Find the DG you want to add the external user to, and select it to open the edit dialog.</span></span>
    
    3. <span data-ttu-id="e7deb-111">Na kartici **članovi** izaberite stavku **Prikaži sve članove**.</span><span class="sxs-lookup"><span data-stu-id="e7deb-111">On the **Members** tab, select **View all and manage members**.</span></span> 
    
    4. <span data-ttu-id="e7deb-112">Izaberite stavku **Dodaj članove**.</span><span class="sxs-lookup"><span data-stu-id="e7deb-112">Select **Add members**.</span></span>
    
    5. <span data-ttu-id="e7deb-113">Izaberite kontakt koji ste kreirali na prethodnom koracima, a zatim izaberite stavku **Sačuvaj**.</span><span class="sxs-lookup"><span data-stu-id="e7deb-113">Select the Mail Contact you created on the previous step, and then select **Save**.</span></span>
    
<span data-ttu-id="e7deb-114">Ako nakon praćenja ovih koraka spoljni korisnici ne mogu da šalju e-poruke na DG ili ne primaju e-poruke iz nje, možda je DG označen tako da omogući e-poruke samo od unutrašnjih korisnika.</span><span class="sxs-lookup"><span data-stu-id="e7deb-114">If after following these steps your external users can't send emails to the DG or don't receive emails from it, it could be that the DG is marked to only allow emails from internal users.</span></span> <span data-ttu-id="e7deb-115">Možete da potvrdite ovu konfiguraciju i da je popravite posle uputstva [ovde](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).</span><span class="sxs-lookup"><span data-stu-id="e7deb-115">You can check this configuration and fix it following the directions [here](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).</span></span>
  
 <span data-ttu-id="e7deb-116">**Napomena:** Ova uputstva se ne primenjuju ako je tip grupe "Microsoft 365 Group" umesto "grupa za distribuciju".</span><span class="sxs-lookup"><span data-stu-id="e7deb-116">**Note:** These instructions don't apply if your group's type is "Microsoft 365 group" instead of "Distribution group."</span></span> <span data-ttu-id="e7deb-117">Ako je to slučaj, možete da dodate spoljnog korisnika direktno u grupu iz programa Outlook.</span><span class="sxs-lookup"><span data-stu-id="e7deb-117">If that is the case, you can add the external user directly to the group from Outlook.</span></span> <span data-ttu-id="e7deb-118">Detaljne informacije o Microsoft 365 grupama gosti, kao i uputstva za dodavanje spoljnih gostiju mogu se pronaći u [ovom članku](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span><span class="sxs-lookup"><span data-stu-id="e7deb-118">Detailed information on Microsoft 365 Groups guests as well as instructions for adding external guests can be found in [this article](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span></span>
  