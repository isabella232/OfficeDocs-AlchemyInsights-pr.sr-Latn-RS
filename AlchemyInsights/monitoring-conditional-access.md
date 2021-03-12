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
ms.custom:
- "9003769"
- "6702"
ms.openlocfilehash: c3bf5dd9066685af2df7ba50f0eb3ba6e891c2a9
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708688"
---
# <a name="monitoring-conditional-access-for-exchange"></a><span data-ttu-id="0bdfa-102">Monitoring uslovnog pristupa za Exchange</span><span class="sxs-lookup"><span data-stu-id="0bdfa-102">Monitoring Conditional Access for Exchange</span></span>

<span data-ttu-id="0bdfa-103">Korisnici koji su usmereni na uslovno pristup dobiće obaveštenje ako ne ispune zahteve za pristup vaše organizacije.</span><span class="sxs-lookup"><span data-stu-id="0bdfa-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="0bdfa-104">Da biste rešili, preporučujemo neka od sledećih rešenja:</span><span class="sxs-lookup"><span data-stu-id="0bdfa-104">To resolve, we recommend one or more of the following solutions:</span></span>

- <span data-ttu-id="0bdfa-105">Ako se na uređaj pretpostavlja da je upisan, savetujte korisnika da ode na aplikaciju portala preduzeća i potvrdi da se pojavljuje na portalu preduzeća.</span><span class="sxs-lookup"><span data-stu-id="0bdfa-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="0bdfa-106">Ako nije, korisnik treba da prijavi uređaj.</span><span class="sxs-lookup"><span data-stu-id="0bdfa-106">If it doesn't, the user should enroll the device.</span></span>
- <span data-ttu-id="0bdfa-107">U Azure portalu idite u Intune > usaglašenost uređaja.</span><span class="sxs-lookup"><span data-stu-id="0bdfa-107">In the Azure portal go to Intune > Device compliance.</span></span> <span data-ttu-id="0bdfa-108">U okviru prati izaberite stavku usaglašenost uređaja.</span><span class="sxs-lookup"><span data-stu-id="0bdfa-108">Under Monitor click Device compliance.</span></span> <span data-ttu-id="0bdfa-109">Prikažite izveštaj usaglašenosti uređaja da biste potvrdili da je uređaj korisnika označen kao usaglašeni.</span><span class="sxs-lookup"><span data-stu-id="0bdfa-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span>
- <span data-ttu-id="0bdfa-110">U Azure portalu idite u Intune > usaglašenost uređaja.</span><span class="sxs-lookup"><span data-stu-id="0bdfa-110">In the Azure portal go to Intune > Device compliance.</span></span> <span data-ttu-id="0bdfa-111">U okviru upravljanje izaberite stavku smernice.</span><span class="sxs-lookup"><span data-stu-id="0bdfa-111">Under Manage, click Policies.</span></span> <span data-ttu-id="0bdfa-112">Na listi smernica usaglašenosti proverite da li je profil dodeljen vašem uređaju.</span><span class="sxs-lookup"><span data-stu-id="0bdfa-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="0bdfa-113">Ako nijedan profil nije dodeljen, Intune neće moći da potvrdi status usaglašenosti uređaja.</span><span class="sxs-lookup"><span data-stu-id="0bdfa-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span>
- <span data-ttu-id="0bdfa-114">Uredite zadatak korisnika uslovnog pristupa.</span><span class="sxs-lookup"><span data-stu-id="0bdfa-114">Edit the user's conditional access assignment.</span></span>

1. <span data-ttu-id="0bdfa-115">U Azure portalu idite na **Podešavanje**  >  **uslovnih**  >  **smernica** za pristup.</span><span class="sxs-lookup"><span data-stu-id="0bdfa-115">In the Azure portal go to **Intune** > **Conditional access** > **Policies**.</span></span>
2. <span data-ttu-id="0bdfa-116">Izaberite smernice sa liste.</span><span class="sxs-lookup"><span data-stu-id="0bdfa-116">Select a policy from the list.</span></span>
3. <span data-ttu-id="0bdfa-117">Izaberite stavku korisnici i grupe.</span><span class="sxs-lookup"><span data-stu-id="0bdfa-117">Click Users and groups.</span></span>
4. <span data-ttu-id="0bdfa-118">Da biste nekome ciljali određenu politiku, dodajte ih na listu "ukljuci".</span><span class="sxs-lookup"><span data-stu-id="0bdfa-118">To target a certain policy at someone, add them to the Include list.</span></span> <span data-ttu-id="0bdfa-119">Da biste se uverili da je osoba izostavljena iz smernica, dodajte ih na listu "Isključi".</span><span class="sxs-lookup"><span data-stu-id="0bdfa-119">To ensure that a person is omitted from the policy, add them to the Exclude list.</span></span>

<span data-ttu-id="0bdfa-120">Korisne veze:</span><span class="sxs-lookup"><span data-stu-id="0bdfa-120">Helpful links:</span></span>

[<span data-ttu-id="0bdfa-121">Pregled usaglašenosti uređaja</span><span class="sxs-lookup"><span data-stu-id="0bdfa-121">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)

[<span data-ttu-id="0bdfa-122">Rešavanje problema sa kom</span><span class="sxs-lookup"><span data-stu-id="0bdfa-122">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[<span data-ttu-id="0bdfa-123">Smernice za rešavanje problema</span><span class="sxs-lookup"><span data-stu-id="0bdfa-123">Troubleshooting policy</span></span>](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

[<span data-ttu-id="0bdfa-124">Nadgledanje usaglašenosti uređaja</span><span class="sxs-lookup"><span data-stu-id="0bdfa-124">Monitoring Intune device compliance</span></span>](https://docs.microsoft.com/intune/compliance-policy-monitor)

<span data-ttu-id="0bdfa-125">Napomena: Ovi koraci su korisni samo u rešavanju problema sa funkcijom Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="0bdfa-125">Note: these steps are only helpful in troubleshooting the Azure Active Directory feature Conditional Access.</span></span> <span data-ttu-id="0bdfa-126">Uređaj može da blokira i blokiranje pristupa e-poštom pomoću Exchange smernica.</span><span class="sxs-lookup"><span data-stu-id="0bdfa-126">It is also possible to quarantine a device blocking it's email access with Exchange policy.</span></span> <span data-ttu-id="0bdfa-127">Više informacija o upravljanju Exchange uređajima može se pronaći [ovde] ( https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141) .</span><span class="sxs-lookup"><span data-stu-id="0bdfa-127">More information on Exchange device management can be found [here](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141).</span></span>
