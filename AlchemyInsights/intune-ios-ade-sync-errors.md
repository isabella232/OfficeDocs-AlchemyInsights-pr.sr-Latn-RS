---
title: Funkcija Apple automatskih upisivanja uređaja
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000654"
- "7256"
ms.openlocfilehash: 912c9e56b4c468fb333769f15bd7c212594dc11a
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/04/2021
ms.locfileid: "50448936"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a><span data-ttu-id="4c75d-102">Funkcija Apple automatskih upisivanja uređaja</span><span class="sxs-lookup"><span data-stu-id="4c75d-102">Apple Automatic Device Enrollment sync errors</span></span>

<span data-ttu-id="4c75d-103">"Otkrili smo da imate neke EJD/DEP simbole koji se nalaze u stanju greške.</span><span class="sxs-lookup"><span data-stu-id="4c75d-103">“We have detected that you have one or more ADE/DEP Tokens which are in an error state.</span></span> <span data-ttu-id="4c75d-104">Dok se stanje greške ne reši za svaki utiču na Token, funkcionalnost Jade neće funkcionisati na očekivani način. ".</span><span class="sxs-lookup"><span data-stu-id="4c75d-104">Until the error state is resolved for each affected token, the ADE functionality will not work as expected.”.</span></span>

<span data-ttu-id="4c75d-105">Ova greška se može manifestuiti na više načina uključujući:</span><span class="sxs-lookup"><span data-stu-id="4c75d-105">This error might manifest in a number of ways including:</span></span>

1. <span data-ttu-id="4c75d-106">Uređaji se možda neće sinhronizovati sa ABM/Jumom u Intune</span><span class="sxs-lookup"><span data-stu-id="4c75d-106">Devices may not sync from ABM/ASM to Intune</span></span>
2. <span data-ttu-id="4c75d-107">Dodeljene profile profila možda neće uspeti</span><span class="sxs-lookup"><span data-stu-id="4c75d-107">Enrollment profile assignments may be failing</span></span>
3. <span data-ttu-id="4c75d-108">Uređaji možda neće uspješno dovršiti prijavljivanje</span><span class="sxs-lookup"><span data-stu-id="4c75d-108">Devices may not complete ADE enrollment successfully</span></span>

<span data-ttu-id="4c75d-109">Potvrdite izbor u vidu greške pri sinhronizaciji prijavljene u konzoli Intune u okviru **Uređaji > Enroll uređaji > Apple prijavljivanje > tokena programa** za prijavljivanje.</span><span class="sxs-lookup"><span data-stu-id="4c75d-109">Check for the sync error reported in the Intune console under **Devices > Enroll Devices > Apple enrollment > Enrollment program tokens**.</span></span>

<span data-ttu-id="4c75d-110">Jedan od najčešćih uzroka greške pri sinhronizaciji je isticanje trenutnog simbola.</span><span class="sxs-lookup"><span data-stu-id="4c75d-110">One of the most common causes of sync error is expiration of the current token.</span></span> <span data-ttu-id="4c75d-111">U mnogim slučajevima, obnavljanje pogođene oznake rešavaće problem.</span><span class="sxs-lookup"><span data-stu-id="4c75d-111">In many cases,renewal of the affected token will resolve the issue.</span></span>

<span data-ttu-id="4c75d-112">Ako je neki od svojih željena istekao, pogledajte sledeću dokumentaciju koja će vam pomoći da ih obnovite po potrebi:</span><span class="sxs-lookup"><span data-stu-id="4c75d-112">If one or more of your tokens has expired,  see the following documentation to help you renew them as appropriate:</span></span>

[<span data-ttu-id="4c75d-113">Obnavljanje simbola automatizovanog upisivanja uređaja</span><span class="sxs-lookup"><span data-stu-id="4c75d-113">Renew an Automated Device Enrollment token</span></span>](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment-program-enroll-ios#renew-an-automated-device-enrollment-token)

<span data-ttu-id="4c75d-114">Pored toga, možete da vidite sledeću dokumentaciju da biste videli potencijalne probleme za druge greške koji prouzrokuju greške simbola:</span><span class="sxs-lookup"><span data-stu-id="4c75d-114">In addition, you can see the following documentation to see potential remediations for other errors causing token synchronization failures:</span></span>

[<span data-ttu-id="4c75d-115">Greške u sinhronizaciji ABM/Zamsync za iOS/iPadOS i macOS automatski Naupisivanje uređaja</span><span class="sxs-lookup"><span data-stu-id="4c75d-115">ABM/ASM Sync Errors for iOS/iPadOS and macOS Automated Device Enrollment Tokens</span></span>](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#sync-token-errors-between-intune-and-ade-dep)







[<span data-ttu-id="4c75d-116">Greške u sinhronizaciji ABM/Zamsync za iOS/iPadOS i macOS automatski Naupisivanje uređaja</span><span class="sxs-lookup"><span data-stu-id="4c75d-116">ABM/ASM Sync Errors for iOS/iPadOS and macOS Automated Device Enrollment Tokens</span></span>](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
