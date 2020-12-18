---
title: Funkcija Apple automatskih upisivanja uređaja
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000654"
- "7256"
ms.openlocfilehash: d7a9398046a1073e30fdbe2950f750bb55d4fa2f
ms.sourcegitcommit: 87c8d0a1e6668211b9dd5427f98984ccdcadb02d
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 12/17/2020
ms.locfileid: "49714977"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a><span data-ttu-id="cd50f-102">Funkcija Apple automatskih upisivanja uređaja</span><span class="sxs-lookup"><span data-stu-id="cd50f-102">Apple Automatic Device Enrollment sync errors</span></span>

<span data-ttu-id="cd50f-103">"Otkrili smo da imate neke EJD/DEP simbole koji se nalaze u stanju greške.</span><span class="sxs-lookup"><span data-stu-id="cd50f-103">“We have detected that you have one or more ADE/DEP Tokens which are in an error state.</span></span> <span data-ttu-id="cd50f-104">Dok se stanje greške ne reši za svaki utiču na Token, funkcionalnost EJD neće funkcionisati na isti način ".</span><span class="sxs-lookup"><span data-stu-id="cd50f-104">Until the error state is resolved for each affected token, the ADE functionality will not work for the same”.</span></span>

<span data-ttu-id="cd50f-105">Ova greška se može manifestuiti na više načina uključujući:</span><span class="sxs-lookup"><span data-stu-id="cd50f-105">This error might manifest in a number of ways including:</span></span>

1. <span data-ttu-id="cd50f-106">Uređaji se možda neće sinhronizovati sa ABM/Jumom u Intune</span><span class="sxs-lookup"><span data-stu-id="cd50f-106">Devices may not sync from ABM/ASM to Intune</span></span>
2. <span data-ttu-id="cd50f-107">Dodeljene profile profila možda neće uspeti</span><span class="sxs-lookup"><span data-stu-id="cd50f-107">Enrollment profile assignments may be failing</span></span>
3. <span data-ttu-id="cd50f-108">Uređaji možda neće uspješno dovršiti prijavljivanje</span><span class="sxs-lookup"><span data-stu-id="cd50f-108">Devices may not complete ADE enrollment successfully</span></span>

<span data-ttu-id="cd50f-109">Proverite da li je došlo do greške pri sinhronizaciji prijavljene u konzoli Intune u okviru **uređaji > Enroll uređajima > Apple prijavljivanje >** inrouacije programa za prijavljivanje i Redigujte sledeću dokumentaciju da biste videli bilo koji potencijalni sistem oporavka:</span><span class="sxs-lookup"><span data-stu-id="cd50f-109">Check for the sync error reported in the Intune console under **Devices > Enroll Devices > Apple enrollment > Enrollment program tokens** and review the following documentation to see any potential remediation:</span></span>

[<span data-ttu-id="cd50f-110">Greške u sinhronizaciji ABM/Zamsync za iOS/iPadOS i macOS automatski Naupisivanje uređaja</span><span class="sxs-lookup"><span data-stu-id="cd50f-110">ABM/ASM Sync Errors for iOS/iPadOS and macOS Automated Device Enrollment Tokens</span></span>](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
