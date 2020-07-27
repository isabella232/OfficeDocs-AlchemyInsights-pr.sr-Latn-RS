---
title: Smernice za zaštitu aplikacija
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/22/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1073"
- "6700006"
ms.openlocfilehash: 7fed65e6749f72e6264070b360a52e72968fc8da
ms.sourcegitcommit: 6f7cbf1dc28c0693009ddf03d9768c1c65018964
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 07/22/2020
ms.locfileid: "45423962"
---
# <a name="application-protection-policy"></a><span data-ttu-id="4468f-102">Smernice za zaštitu aplikacija</span><span class="sxs-lookup"><span data-stu-id="4468f-102">Application protection policy</span></span>

<span data-ttu-id="4468f-103">Ako ste novi u smernicama za zaštitu aplikacija (aplikacija), pogledajte [Pregled smernica zaštite aplikacija](https://docs.microsoft.com/intune/apps/app-protection-policy).</span><span class="sxs-lookup"><span data-stu-id="4468f-103">If you're new to Application protection policy (APP), check out the [App protection policies overview](https://docs.microsoft.com/intune/apps/app-protection-policy).</span></span>

<span data-ttu-id="4468f-104">Da biste počeli da koristite aplikaciju, pogledajte [Kako da kreirate i dodelite smernice za zaštitu aplikacija](https://docs.microsoft.com/intune/app-protection-policies).</span><span class="sxs-lookup"><span data-stu-id="4468f-104">To start using APP, see [How to create and assign app protection policies](https://docs.microsoft.com/intune/app-protection-policies).</span></span>

<span data-ttu-id="4468f-105">Zahtevi smernica za zaštitu aplikacija:</span><span class="sxs-lookup"><span data-stu-id="4468f-105">Application protection policy requirements:</span></span>

- <span data-ttu-id="4468f-106">Korisnik ima licencu za Intune ili EMS.</span><span class="sxs-lookup"><span data-stu-id="4468f-106">User has an Intune or EMS license.</span></span>
- <span data-ttu-id="4468f-107">Korisnik pripada grupi smernicama za zaštitu aplikacija.</span><span class="sxs-lookup"><span data-stu-id="4468f-107">User belongs to a group targeted by application protection policies.</span></span>
- <span data-ttu-id="4468f-108">Samo jedan korporativni korisnik je prijavljen u zaštićene aplikacije na uređaju.</span><span class="sxs-lookup"><span data-stu-id="4468f-108">Only one corporate user is signed into protected apps on a device.</span></span>
- <span data-ttu-id="4468f-109">Aplikacija je sprovela program [INTUNE SDK](https://docs.microsoft.com/intune/app-sdk-get-started).</span><span class="sxs-lookup"><span data-stu-id="4468f-109">The application has implemented the [Intune SDK](https://docs.microsoft.com/intune/app-sdk-get-started).</span></span> <span data-ttu-id="4468f-110">Da biste dobili listu aplikacija koje podržavaju SDK, pogledajte [Microsoft Intune zaštićene aplikacije](https://docs.microsoft.com/intune/apps-supported-intune-apps).</span><span class="sxs-lookup"><span data-stu-id="4468f-110">For a list of apps that support the SDK, see [Microsoft Intune protected apps](https://docs.microsoft.com/intune/apps-supported-intune-apps).</span></span>

<span data-ttu-id="4468f-111">Smernice se primenjuju nakon što korisnik koji zadovoljava gorenavedene zahteve prijavljuje u aplikaciju "Intune" omogućenu za SDK.</span><span class="sxs-lookup"><span data-stu-id="4468f-111">Policies apply after a user who meets the above requirements signs into an Intune SDK enabled app.</span></span> <span data-ttu-id="4468f-112">Najlakši način da utvrdite da li su smernice primenjene je tako što ćete zahtevati da korisnik Postavi PIN u smernice.</span><span class="sxs-lookup"><span data-stu-id="4468f-112">The easiest way to determine if a policy is applied is by requiring that the user set a pin in the policy.</span></span> 

<span data-ttu-id="4468f-113">Za više informacija pogledajte članak:</span><span class="sxs-lookup"><span data-stu-id="4468f-113">For more information, see:</span></span>

[<span data-ttu-id="4468f-114">Najčešća pitanja o rešavanju problema sa APLIKACIJOM/MAM</span><span class="sxs-lookup"><span data-stu-id="4468f-114">APP/MAM troubleshooting FAQ</span></span>](https://docs.microsoft.com/intune/apps/troubleshoot-mam)  

[<span data-ttu-id="4468f-115">Provera valjanosti podešavanja smernica za zaštitu aplikacija</span><span class="sxs-lookup"><span data-stu-id="4468f-115">How to validate your app protection policy setup</span></span>](https://docs.microsoft.com/intune/app-protection-policies-validate)

[<span data-ttu-id="4468f-116">Razumevanje vremena isporuke smernica za zaštitu aplikacija</span><span class="sxs-lookup"><span data-stu-id="4468f-116">Understand App Protection Policy delivery timing</span></span>](https://docs.microsoft.com/intune/app-protection-policy-delivery)  

[<span data-ttu-id="4468f-117">Kako nadgledati smernice za zaštitu aplikacija?</span><span class="sxs-lookup"><span data-stu-id="4468f-117">How to monitor app protection policies</span></span>](https://docs.microsoft.com/intune/app-protection-policies-monitor)