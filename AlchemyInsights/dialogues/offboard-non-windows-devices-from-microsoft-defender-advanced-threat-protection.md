---
title: Office uređaji koji nisu Windows uređaji iz napredne zaštite pretnje Microsoft Defender (ATP)
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 435957c555cd80155a985a49bd94b041a4ada31d
ms.sourcegitcommit: 4883f1f89d4c6ca23161e9a43ff206ad21d4f09b
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/08/2021
ms.locfileid: "50695158"
---
# <a name="offboard-non-windows-devices-from-microsoft-defender-advanced-threat-protection-atp"></a><span data-ttu-id="e7a0b-102">Office uređaji koji nisu Windows uređaji iz napredne zaštite pretnje Microsoft Defender (ATP)</span><span class="sxs-lookup"><span data-stu-id="e7a0b-102">Offboard non-Windows devices from Microsoft Defender Advanced Threat Protection (ATP)</span></span>

<span data-ttu-id="e7a0b-103">Evo kako:</span><span class="sxs-lookup"><span data-stu-id="e7a0b-103">Here's how:</span></span>

1. <span data-ttu-id="e7a0b-104">Potražite samostalnu dokumentaciju za prekid povezivanja nezavisnog rešenja iz ATP-a.</span><span class="sxs-lookup"><span data-stu-id="e7a0b-104">Follow the third-party documentation for disconnecting the third-party solution from Microsoft Defender ATP.</span></span>
2. <span data-ttu-id="e7a0b-105">Iz Azure Active Directory stanara, uklonite dozvole za rešenje nezavisnog proizvođača:</span><span class="sxs-lookup"><span data-stu-id="e7a0b-105">From your Azure Active Directory tenant, remove permissions for the third-party solution:</span></span>

    1. <span data-ttu-id="e7a0b-106">Prijavite se na [Azure portal](https://go.microsoft.com/fwlink/?linkid=2125612).</span><span class="sxs-lookup"><span data-stu-id="e7a0b-106">Sign in to the [Azure portal](https://go.microsoft.com/fwlink/?linkid=2125612).</span></span>
    1. <span data-ttu-id="e7a0b-107">Izaberite stavku **sve usluge**  >  **Azure Active Directory**  >  **Enterprise aplikacije**.</span><span class="sxs-lookup"><span data-stu-id="e7a0b-107">Select **All services** > **Azure Active Directory** > **Enterprise Applications**.</span></span>
    1. <span data-ttu-id="e7a0b-108">Izaberite aplikaciju koju želite da skinete.</span><span class="sxs-lookup"><span data-stu-id="e7a0b-108">Select the application you'd like to offboard.</span></span>
    1. <span data-ttu-id="e7a0b-109">Izaberite stavku **Izbriši**.</span><span class="sxs-lookup"><span data-stu-id="e7a0b-109">Select **Delete**.</span></span>

<span data-ttu-id="e7a0b-110">Da biste saznali više, pogledajte članak [Odbord ne-Windows uređajima](https://go.microsoft.com/fwlink/?linkid=2143630).</span><span class="sxs-lookup"><span data-stu-id="e7a0b-110">To learn more, see [Offboard non-Windows devices](https://go.microsoft.com/fwlink/?linkid=2143630).</span></span>
