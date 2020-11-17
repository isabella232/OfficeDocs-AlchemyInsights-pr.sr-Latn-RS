---
title: Kreiranje grupe
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003234"
- "7230"
ms.openlocfilehash: b8cb3f1de991bfe7197607d5e8964a018e31c122
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 11/17/2020
ms.locfileid: "49089174"
---
# <a name="create-a-group"></a><span data-ttu-id="a5ae3-102">Kreiranje grupe</span><span class="sxs-lookup"><span data-stu-id="a5ae3-102">Create a group</span></span>

<span data-ttu-id="a5ae3-103">Ova tema opisuje Kreiranje grupe.</span><span class="sxs-lookup"><span data-stu-id="a5ae3-103">This topic describes group creation.</span></span>

<span data-ttu-id="a5ae3-104">**Dozvola za kreiranje grupe**</span><span class="sxs-lookup"><span data-stu-id="a5ae3-104">**Permission to Create a Group**</span></span>

<span data-ttu-id="a5ae3-105">Uverite se da ste ovlašćeni za kreiranje nove grupe.</span><span class="sxs-lookup"><span data-stu-id="a5ae3-105">Ensure you are authorized to create a new group.</span></span> <span data-ttu-id="a5ae3-106">Globalni administratori mogu da onemoguće Kreiranje grupe na Azure portovu ili Access tabli.</span><span class="sxs-lookup"><span data-stu-id="a5ae3-106">Global administrators can disable group creation in the Azure portal or Access Panel.</span></span> <span data-ttu-id="a5ae3-107">Možda će vam biti potreban administrator da biste kreirali novu grupu za vas ili da biste vam dali odgovarajuće dozvole.</span><span class="sxs-lookup"><span data-stu-id="a5ae3-107">You may need an administrator to create the new group for you, or to give you appropriate permissions.</span></span>

<span data-ttu-id="a5ae3-108">**Upravljanje dozvolama za kreiranje grupe**</span><span class="sxs-lookup"><span data-stu-id="a5ae3-108">**Manage Group creation permissions**</span></span>

1. <span data-ttu-id="a5ae3-109">Globalni administratori mogu da upravljaju dozvolama za kreiranje grupe (iz bezbednosnih razloga) ili Office 365 grupama kreirane na Azure portovi ili Access tabli, tako što ćete izabrati "korisnici mogu da kreiraju bezbednosne grupe u Azure portali" ili "korisnici mogu da kreiraju Office 365 grupe u Azure portali" **All groups**  >  **(postavke)**.</span><span class="sxs-lookup"><span data-stu-id="a5ae3-109">Global administrators can manage group creation permissions (for security-related reasons) or Office 365 groups created in the Azure portal or Access Panel, by choosing "Users can create security groups in Azure portals" or "Users can create Office 365 groups in Azure portals" options in **All groups** > **General (Settings)**.</span></span>
2. <span data-ttu-id="a5ae3-110">Možete i da ograničite Kreiranje grupe da biste izabrali grupu korisnika ako imate licencu za Azure Active Directory P1 Premium.</span><span class="sxs-lookup"><span data-stu-id="a5ae3-110">You can also restrict group creation to select a group of users if you have an Azure Active Directory P1 Premium license.</span></span>

<span data-ttu-id="a5ae3-111">**Onemogućavanje obaveštenja o dobrodošlici za nove Office 365 članove grupe**</span><span class="sxs-lookup"><span data-stu-id="a5ae3-111">**Disabling welcome notification for new Office 365 group members**</span></span>

<span data-ttu-id="a5ae3-112">Obaveštenje o dobrodošlici koje se šalju korisnicima koji se dodaju u Office 365 grupe mogu da se onemogućavaju postavljanjem **sindikalnog polja omogućeno** u PowerShell.</span><span class="sxs-lookup"><span data-stu-id="a5ae3-112">The welcome notification sent to users who are added to Office 365 groups can be disabled by setting **UnifiedGroupWelcomeMessageEnabled** to False in Powershell.</span></span> <span data-ttu-id="a5ae3-113">Saznajte više o ovoj podešavanju [ovde](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="a5ae3-113">Learn about this setting [here](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).</span></span>

