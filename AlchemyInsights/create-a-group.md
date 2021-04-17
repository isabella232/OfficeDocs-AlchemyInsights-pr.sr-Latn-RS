---
title: Kreiranje grupe
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003234"
- "7230"
ms.openlocfilehash: ec74b7c098d302d3bdeb5a412fad41efe7b82b98
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816375"
---
# <a name="create-a-group"></a><span data-ttu-id="b0ea4-102">Kreiranje grupe</span><span class="sxs-lookup"><span data-stu-id="b0ea4-102">Create a group</span></span>

<span data-ttu-id="b0ea4-103">Ova tema opisuje kreiranje grupa.</span><span class="sxs-lookup"><span data-stu-id="b0ea4-103">This topic describes group creation.</span></span>

<span data-ttu-id="b0ea4-104">**Dozvola za kreiranje grupe**</span><span class="sxs-lookup"><span data-stu-id="b0ea4-104">**Permission to Create a Group**</span></span>

<span data-ttu-id="b0ea4-105">Uverite se da ste ovlašćeni za kreiranje nove grupe.</span><span class="sxs-lookup"><span data-stu-id="b0ea4-105">Ensure you are authorized to create a new group.</span></span> <span data-ttu-id="b0ea4-106">Globalni administratori mogu da onemoguće kreiranje grupa na Azure portalu ili na Access tabli.</span><span class="sxs-lookup"><span data-stu-id="b0ea4-106">Global administrators can disable group creation in the Azure portal or Access Panel.</span></span> <span data-ttu-id="b0ea4-107">Možda će vam biti potreban administrator da biste napravili novu grupu za vas ili da bi vam dao odgovarajuće dozvole.</span><span class="sxs-lookup"><span data-stu-id="b0ea4-107">You may need an administrator to create the new group for you, or to give you appropriate permissions.</span></span>

<span data-ttu-id="b0ea4-108">**Upravljanje dozvolama za kreiranje grupe**</span><span class="sxs-lookup"><span data-stu-id="b0ea4-108">**Manage Group creation permissions**</span></span>

1. <span data-ttu-id="b0ea4-109">Globalni administratori mogu da upravljaju dozvolama za kreiranje grupa (iz bezbednosnih razloga) ili Office 365 grupama kreiranim na Azure portalu ili na tabli za pristup, tako što će u opcijama "Korisnici mogu da kreiraju bezbednosne grupe na Azure portalima" ili "Korisnici mogu da kreiraju Office 365 grupe na Azure portalima" u opcijama Sve grupe Opšte  >  **(Postavke).**</span><span class="sxs-lookup"><span data-stu-id="b0ea4-109">Global administrators can manage group creation permissions (for security-related reasons) or Office 365 groups created in the Azure portal or Access Panel, by choosing "Users can create security groups in Azure portals" or "Users can create Office 365 groups in Azure portals" options in **All groups** > **General (Settings)**.</span></span>
2. <span data-ttu-id="b0ea4-110">Možete i da ograničite kreiranje grupa da biste izabrali grupu korisnika ako imate Azure Active Directory P1 Premium licencu.</span><span class="sxs-lookup"><span data-stu-id="b0ea4-110">You can also restrict group creation to select a group of users if you have an Azure Active Directory P1 Premium license.</span></span>

<span data-ttu-id="b0ea4-111">**Kako da neometano obaveštenje o dobrodošlici za nove članove Office 365 grupe**</span><span class="sxs-lookup"><span data-stu-id="b0ea4-111">**Disabling welcome notification for new Office 365 group members**</span></span>

<span data-ttu-id="b0ea4-112">Obaveštenje dobrodošlice poslato korisnicima koji su dodati u Office 365 grupe može se onemogućiti postavljanjem **funkcije UnifiedGroupWelcomeMessageEnabled** na False u programu PowerShell.</span><span class="sxs-lookup"><span data-stu-id="b0ea4-112">The welcome notification sent to users who are added to Office 365 groups can be disabled by setting **UnifiedGroupWelcomeMessageEnabled** to False in Powershell.</span></span> <span data-ttu-id="b0ea4-113">Više o ovoj postavki [saznajte ovde.](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true)</span><span class="sxs-lookup"><span data-stu-id="b0ea4-113">Learn about this setting [here](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).</span></span>

