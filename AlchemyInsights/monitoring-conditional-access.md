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
ms.openlocfilehash: 0687875a3714067e774872d02630564858d71d1b
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 10/06/2020
ms.locfileid: "48366442"
---
# <a name="monitoring-conditional-access-for-exchange"></a><span data-ttu-id="a06f2-102">Monitoring uslovnog pristupa za Exchange</span><span class="sxs-lookup"><span data-stu-id="a06f2-102">Monitoring Conditional Access for Exchange</span></span>

<span data-ttu-id="a06f2-103">Korisnici koji su usmereni na uslovno pristup dobiće obaveštenje ako ne ispune zahteve za pristup vaše organizacije.</span><span class="sxs-lookup"><span data-stu-id="a06f2-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="a06f2-104">Da biste rešili, preporučujemo neka od sledećih rešenja:</span><span class="sxs-lookup"><span data-stu-id="a06f2-104">To resolve, we recommend one or more of the following solutions:</span></span>

- <span data-ttu-id="a06f2-105">Ako se na uređaj pretpostavlja da je upisan, savetujte korisnika da ode na aplikaciju portala preduzeća i potvrdi da se pojavljuje na portalu preduzeća.</span><span class="sxs-lookup"><span data-stu-id="a06f2-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="a06f2-106">Ako nije, korisnik treba da prijavi uređaj.</span><span class="sxs-lookup"><span data-stu-id="a06f2-106">If it doesn't, the user should enroll the device.</span></span>
- <span data-ttu-id="a06f2-107">U Azure portalu idite u Intune > usaglašenost uređaja.</span><span class="sxs-lookup"><span data-stu-id="a06f2-107">In the Azure portal go to Intune > Device compliance.</span></span> <span data-ttu-id="a06f2-108">U okviru prati izaberite stavku usaglašenost uređaja.</span><span class="sxs-lookup"><span data-stu-id="a06f2-108">Under Monitor click Device compliance.</span></span> <span data-ttu-id="a06f2-109">Prikažite izveštaj usaglašenosti uređaja da biste potvrdili da je uređaj korisnika označen kao usaglašeni.</span><span class="sxs-lookup"><span data-stu-id="a06f2-109">View your device compliance report to verify that the user's device is marked as compliant.</span></span>
- <span data-ttu-id="a06f2-110">U Azure portalu idite u Intune > usaglašenost uređaja.</span><span class="sxs-lookup"><span data-stu-id="a06f2-110">In the Azure portal go to Intune > Device compliance.</span></span> <span data-ttu-id="a06f2-111">U okviru upravljanje izaberite stavku smernice.</span><span class="sxs-lookup"><span data-stu-id="a06f2-111">Under Manage, click Policies.</span></span> <span data-ttu-id="a06f2-112">Na listi smernica usaglašenosti proverite da li je profil dodeljen vašem uređaju.</span><span class="sxs-lookup"><span data-stu-id="a06f2-112">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="a06f2-113">Ako nijedan profil nije dodeljen, Intune neće moći da potvrdi status usaglašenosti uređaja.</span><span class="sxs-lookup"><span data-stu-id="a06f2-113">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span>
- <span data-ttu-id="a06f2-114">Uredite zadatak korisnika uslovnog pristupa.</span><span class="sxs-lookup"><span data-stu-id="a06f2-114">Edit the user's conditional access assignment.</span></span>

1. <span data-ttu-id="a06f2-115">U Azure portalu idite na **Podešavanje**  >  **uslovnih**  >  **smernica**za pristup.</span><span class="sxs-lookup"><span data-stu-id="a06f2-115">In the Azure portal go to **Intune** > **Conditional access** > **Policies**.</span></span>
2. <span data-ttu-id="a06f2-116">Izaberite smernice sa liste.</span><span class="sxs-lookup"><span data-stu-id="a06f2-116">Select a policy from the list.</span></span>
3. <span data-ttu-id="a06f2-117">Izaberite stavku korisnici i grupe.</span><span class="sxs-lookup"><span data-stu-id="a06f2-117">Click Users and groups.</span></span>
4. <span data-ttu-id="a06f2-118">Da biste nekome ciljali određenu politiku, dodajte ih na listu "ukljuci".</span><span class="sxs-lookup"><span data-stu-id="a06f2-118">To target a certain policy at someone, add them to the Include list.</span></span> <span data-ttu-id="a06f2-119">Da biste se uverili da je osoba izostavljena iz smernica, dodajte ih na listu "Isključi".</span><span class="sxs-lookup"><span data-stu-id="a06f2-119">To ensure that a person is omitted from the policy, add them to the Exclude list.</span></span>

<span data-ttu-id="a06f2-120">Korisne veze:</span><span class="sxs-lookup"><span data-stu-id="a06f2-120">Helpful links:</span></span>

[<span data-ttu-id="a06f2-121">Pregled usaglašenosti uređaja</span><span class="sxs-lookup"><span data-stu-id="a06f2-121">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)

[<span data-ttu-id="a06f2-122">Rešavanje problema sa kom</span><span class="sxs-lookup"><span data-stu-id="a06f2-122">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[<span data-ttu-id="a06f2-123">Smernice za rešavanje problema</span><span class="sxs-lookup"><span data-stu-id="a06f2-123">Troubleshooting policy</span></span>](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

[<span data-ttu-id="a06f2-124">Nadgledanje usaglašenosti uređaja</span><span class="sxs-lookup"><span data-stu-id="a06f2-124">Monitoring Intune device compliance</span></span>](https://docs.microsoft.com/intune/compliance-policy-monitor)

<span data-ttu-id="a06f2-125">Napomena: Ovi koraci su korisni samo u rešavanju problema sa funkcijom Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="a06f2-125">Note: these steps are only helpful in troubleshooting the Azure Active Directory feature Conditional Access.</span></span> <span data-ttu-id="a06f2-126">Uređaj može da blokira i blokiranje pristupa e-poštom pomoću Exchange smernica.</span><span class="sxs-lookup"><span data-stu-id="a06f2-126">It is also possible to quarantine a device blocking it's email access with Exchange policy.</span></span> <span data-ttu-id="a06f2-127">Više informacija o upravljanju Exchange uređajima možete da pronađete [ovde](<https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141>).</span><span class="sxs-lookup"><span data-stu-id="a06f2-127">More information on Exchange device management can be found [here](<https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141>).</span></span>
