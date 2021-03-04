---
title: Nadgledanje uslovnog pristupa
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004636"
- "8386"
ms.openlocfilehash: e2803a49aaf087ac55b1fd62056e2b0af3fcd919
ms.sourcegitcommit: 229bd519ec1c14c65a243226a94eee23e117a7fc
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/03/2021
ms.locfileid: "50428313"
---
# <a name="monitor-intune-conditional-access"></a><span data-ttu-id="b6d96-102">Nadgledanje uslovnog pristupa</span><span class="sxs-lookup"><span data-stu-id="b6d96-102">Monitor Intune Conditional Access</span></span>

<span data-ttu-id="b6d96-103">Korisnici koji su usmereni na uslovno pristup dobiće obaveštenje ako ne ispune zahteve za pristup vaše organizacije.</span><span class="sxs-lookup"><span data-stu-id="b6d96-103">Users targeted with conditional access will receive a notification email if they do not meet your organization's access requirements.</span></span> <span data-ttu-id="b6d96-104">Da biste rešili, preporučujemo neka od sledećih rešenja:</span><span class="sxs-lookup"><span data-stu-id="b6d96-104">To resolve, we recommend one or more of the following solutions:</span></span>

1. <span data-ttu-id="b6d96-105">Ako se na uređaj pretpostavlja da je upisan, savetujte korisnika da ode na aplikaciju portala preduzeća i potvrdi da se pojavljuje na portalu preduzeća.</span><span class="sxs-lookup"><span data-stu-id="b6d96-105">If the device is presumed to be enrolled, advise the user to go to the Company Portal app and verify that it appears in the Company Portal.</span></span> <span data-ttu-id="b6d96-106">Ako nije, korisnik mora da prijavi uređaj.</span><span class="sxs-lookup"><span data-stu-id="b6d96-106">If it doesn't, the user must enroll the device.</span></span>
1. <span data-ttu-id="b6d96-107">U Azure portalu **Idite na**  >  **usaglašenost uređaja**.</span><span class="sxs-lookup"><span data-stu-id="b6d96-107">In the Azure portal go to **Intune** > **Device compliance**.</span></span> 
1. <span data-ttu-id="b6d96-108">Da biste videli izveštaj o usaglašenosti uređaja da biste proverili da li je uređaj za korisnike označen kao usaglašeni, u okviru **monitor** izaberite stavku **usaglašenost uređaja**.</span><span class="sxs-lookup"><span data-stu-id="b6d96-108">To view your device compliance report to verify that the user's device is marked as compliant, under **Monitor**, click **Device compliance**.</span></span>
1. <span data-ttu-id="b6d96-109">U Azure portalu **Idite na**  >  **usaglašenost uređaja**.</span><span class="sxs-lookup"><span data-stu-id="b6d96-109">In the Azure portal go to **Intune** > **Device compliance**.</span></span> <span data-ttu-id="b6d96-110">U okviru **Upravljanje** izaberite stavku **smernice**.</span><span class="sxs-lookup"><span data-stu-id="b6d96-110">Under **Manage,** click **Policies**.</span></span> <span data-ttu-id="b6d96-111">Na listi smernica usaglašenosti proverite da li je profil dodeljen vašem uređaju.</span><span class="sxs-lookup"><span data-stu-id="b6d96-111">In the list of compliance policies, verify that a profile is assigned to your user's device.</span></span> <span data-ttu-id="b6d96-112">Ako nijedan profil nije dodeljen, Intune neće moći da potvrdi status usaglašenosti uređaja.</span><span class="sxs-lookup"><span data-stu-id="b6d96-112">If no profile is assigned, then Intune will not be able to confirm the device's compliance status.</span></span>
1. <span data-ttu-id="b6d96-113">Uredite zadatak korisnika uslovnog pristupa.</span><span class="sxs-lookup"><span data-stu-id="b6d96-113">Edit the user's conditional access assignment.</span></span>
1. <span data-ttu-id="b6d96-114">Na Azure portalu idite da biste **podesili**  >  **uslovne**  >  **smernice** za pristup, izaberite smernice sa liste i izaberite stavku **korisnici i grupe**.</span><span class="sxs-lookup"><span data-stu-id="b6d96-114">In the Azure portal, navigate to **Intune** > **Conditional access** > **Policies**, select a policy from the list, and click **Users and groups**.</span></span>
1. <span data-ttu-id="b6d96-115">Da biste nekome ciljali određenu politiku, dodajte ih na **listu "ukljuci**".</span><span class="sxs-lookup"><span data-stu-id="b6d96-115">To target a certain policy at someone, add them to the **Include list**.</span></span> <span data-ttu-id="b6d96-116">Da biste se uverili da je osoba izostavljena iz smernica, dodajte ih na **listu "Isključi**".</span><span class="sxs-lookup"><span data-stu-id="b6d96-116">To ensure that a person is omitted from the policy, add them to the **Exclude list**.</span></span>

<span data-ttu-id="b6d96-117">**Korisne veze:**</span><span class="sxs-lookup"><span data-stu-id="b6d96-117">**Helpful links:**</span></span>

- [<span data-ttu-id="b6d96-118">Pregled usaglašenosti uređaja</span><span class="sxs-lookup"><span data-stu-id="b6d96-118">Device compliance overview</span></span>](https://docs.microsoft.com/intune/device-compliance-get-started)
- [<span data-ttu-id="b6d96-119">Rešavanje problema sa kom</span><span class="sxs-lookup"><span data-stu-id="b6d96-119">Troubleshooting CA</span></span>](https://docs.microsoft.com/intune/troubleshoot-conditional-access)
- [<span data-ttu-id="b6d96-120">Smernice za rešavanje problema</span><span class="sxs-lookup"><span data-stu-id="b6d96-120">Troubleshooting policy</span></span>](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)
- [<span data-ttu-id="b6d96-121">Nadgledanje usaglašenosti uređaja</span><span class="sxs-lookup"><span data-stu-id="b6d96-121">Monitoring Intune device compliance</span></span>](https://docs.microsoft.com/intune/compliance-policy-monitor)

> [!NOTE]
> <span data-ttu-id="b6d96-122">Ovi koraci su korisni samo u rešavanju problema sa funkcijom Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="b6d96-122">These steps are only helpful in troubleshooting the Azure Active Directory feature Conditional Access.</span></span> <span data-ttu-id="b6d96-123">Uređaj može da blokira i blokiranje pristupa e-poštom pomoću Exchange smernica.</span><span class="sxs-lookup"><span data-stu-id="b6d96-123">It is also possible to quarantine a device blocking it's email access with Exchange policy.</span></span> <span data-ttu-id="b6d96-124">Više informacija o upravljanju Exchange uređajima možete da pronađete [**ovde**](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141)).</span><span class="sxs-lookup"><span data-stu-id="b6d96-124">More information on Exchange device management can be found [**here**](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141)).</span></span>
