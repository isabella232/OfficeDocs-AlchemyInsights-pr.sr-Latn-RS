---
title: Monitoring uslovnog pristupa
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 6083fc427e3791fdb0907198b525337a0c987c4e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47702917"
---
# <a name="monitoring-conditional-access-for-exchange"></a><span data-ttu-id="827b0-102">Monitoring uslovnog pristupa za Exchange</span><span class="sxs-lookup"><span data-stu-id="827b0-102">Monitoring Conditional Access for Exchange</span></span>

<span data-ttu-id="827b0-103">Korisnici koji su usmereni na uslovno pristup dobiće obaveštenje ako ne ispune zahteve za pristup vaše organizacije.</span><span class="sxs-lookup"><span data-stu-id="827b0-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="827b0-104">Da biste rešili, preporučujemo neka od sledećih rešenja:</span><span class="sxs-lookup"><span data-stu-id="827b0-104">To resolve, we recommend one or more of the following solutions:</span></span>
  
- <span data-ttu-id="827b0-105">Ako se na uređaj pretpostavlja da je upisan, savetujte korisnika da ode na aplikaciju portala preduzeća i potvrdi da se pojavljuje na portalu preduzeća.</span><span class="sxs-lookup"><span data-stu-id="827b0-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="827b0-106">Ako nije, korisnik treba da prijavi uređaj.</span><span class="sxs-lookup"><span data-stu-id="827b0-106">If it doesn't, the user should enroll the device.</span></span>
    
- <span data-ttu-id="827b0-107">U Azure portalu idite na \*\* \> usaglašenost uređaja\*\*.</span><span class="sxs-lookup"><span data-stu-id="827b0-107">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="827b0-108">U okviru **prati** izaberite stavku **usaglašenost uređaja**.</span><span class="sxs-lookup"><span data-stu-id="827b0-108">Under **Monitor** click **Device compliance**.</span></span> <span data-ttu-id="827b0-109">Prikažite izveštaj usaglašenosti uređaja da biste potvrdili da je uređaj korisnika označen kao usaglašeni.</span><span class="sxs-lookup"><span data-stu-id="827b0-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span> 
    
- <span data-ttu-id="827b0-110">U Azure portalu idite na \*\* \> usaglašenost uređaja\*\*.</span><span class="sxs-lookup"><span data-stu-id="827b0-110">In the Azure portal go to **Intune \> Device compliance**.</span></span> <span data-ttu-id="827b0-111">U okviru **Upravljanje**izaberite stavku **smernice**.</span><span class="sxs-lookup"><span data-stu-id="827b0-111">Under **Manage**, click **Policies**.</span></span> <span data-ttu-id="827b0-112">Na listi smernica usaglašenosti proverite da li je profil dodeljen vašem uređaju.</span><span class="sxs-lookup"><span data-stu-id="827b0-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="827b0-113">Ako nijedan profil nije dodeljen, Intune neće moći da potvrdi status usaglašenosti uređaja.</span><span class="sxs-lookup"><span data-stu-id="827b0-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span> 
    
- <span data-ttu-id="827b0-114">Uredite zadatak korisnika uslovnog pristupa.</span><span class="sxs-lookup"><span data-stu-id="827b0-114">Edit the user's conditional access assignment.</span></span>
    
1. <span data-ttu-id="827b0-115">U Azure portalu idite na **Podešavanje \> uslovne \> smernice za pristup**</span><span class="sxs-lookup"><span data-stu-id="827b0-115">In the Azure portal go to **Intune \> Conditional access \> Policies**</span></span>
    
2. <span data-ttu-id="827b0-116">Izbor smernica sa liste</span><span class="sxs-lookup"><span data-stu-id="827b0-116">Select a policy from the list</span></span>
    
3. <span data-ttu-id="827b0-117">Izaberite stavku **korisnici i grupe**</span><span class="sxs-lookup"><span data-stu-id="827b0-117">Click **Users and groups**</span></span>
    
4. <span data-ttu-id="827b0-118">Da biste nekome ciljali određenu politiku, dodajte ih na listu " **ukljuci** ".</span><span class="sxs-lookup"><span data-stu-id="827b0-118">To target a certain policy at someone, add them to the **Include** list.</span></span> <span data-ttu-id="827b0-119">Da biste se uverili da je osoba **izostavljena** iz smernica, dodajte ih na listu "Isključi".</span><span class="sxs-lookup"><span data-stu-id="827b0-119">To ensure that a person is omitted from the policy, add them to the **Exclude** list.</span></span> 
    
<span data-ttu-id="827b0-120">Pročitajte više: [kako nadgledati uslovno pristup uređajima](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span><span class="sxs-lookup"><span data-stu-id="827b0-120">Read more: [How to Monitor Conditional Access devices](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)</span></span>
  

