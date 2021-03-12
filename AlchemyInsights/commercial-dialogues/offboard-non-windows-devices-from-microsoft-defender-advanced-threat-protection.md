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
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/11/2021
ms.locfileid: "50748481"
---
# <a name="offboard-non-windows-devices-from-microsoft-defender-advanced-threat-protection-atp"></a><span data-ttu-id="c0ba4-102">Office uređaji koji nisu Windows uređaji iz napredne zaštite pretnje Microsoft Defender (ATP)</span><span class="sxs-lookup"><span data-stu-id="c0ba4-102">Offboard non-Windows devices from Microsoft Defender Advanced Threat Protection (ATP)</span></span>

<span data-ttu-id="c0ba4-103">Evo kako:</span><span class="sxs-lookup"><span data-stu-id="c0ba4-103">Here's how:</span></span>

1. <span data-ttu-id="c0ba4-104">Potražite samostalnu dokumentaciju za prekid povezivanja nezavisnog rešenja iz ATP-a.</span><span class="sxs-lookup"><span data-stu-id="c0ba4-104">Follow the third-party documentation for disconnecting the third-party solution from Microsoft Defender ATP.</span></span>
2. <span data-ttu-id="c0ba4-105">Iz Azure Active Directory stanara, uklonite dozvole za rešenje nezavisnog proizvođača:</span><span class="sxs-lookup"><span data-stu-id="c0ba4-105">From your Azure Active Directory tenant, remove permissions for the third-party solution:</span></span>

    1. <span data-ttu-id="c0ba4-106">Prijavite se na [Azure portal](https://go.microsoft.com/fwlink/?linkid=2125612).</span><span class="sxs-lookup"><span data-stu-id="c0ba4-106">Sign in to the [Azure portal](https://go.microsoft.com/fwlink/?linkid=2125612).</span></span>
    1. <span data-ttu-id="c0ba4-107">Izaberite stavku **sve usluge**  >  **Azure Active Directory**  >  **Enterprise aplikacije**.</span><span class="sxs-lookup"><span data-stu-id="c0ba4-107">Select **All services** > **Azure Active Directory** > **Enterprise Applications**.</span></span>
    1. <span data-ttu-id="c0ba4-108">Izaberite aplikaciju koju želite da skinete.</span><span class="sxs-lookup"><span data-stu-id="c0ba4-108">Select the application you'd like to offboard.</span></span>
    1. <span data-ttu-id="c0ba4-109">Izaberite stavku **Izbriši**.</span><span class="sxs-lookup"><span data-stu-id="c0ba4-109">Select **Delete**.</span></span>

<span data-ttu-id="c0ba4-110">Da biste saznali više, pogledajte članak [Odbord ne-Windows uređajima](https://go.microsoft.com/fwlink/?linkid=2143630).</span><span class="sxs-lookup"><span data-stu-id="c0ba4-110">To learn more, see [Offboard non-Windows devices](https://go.microsoft.com/fwlink/?linkid=2143630).</span></span>
