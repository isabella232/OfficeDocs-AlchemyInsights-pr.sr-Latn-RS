---
title: Problemi sa uklanjanjem rastećeg ili preklonjenog uređaja iz zaliha uređaja
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/11/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002913"
- "11187"
ms.openlocfilehash: 46ac46c583cd0ac956797737d8150277f0d79ba5
ms.sourcegitcommit: c685f197dbf83a9dfd85e9acfdf14a4daf0e9a5a
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 05/11/2021
ms.locfileid: "52564607"
---
# <a name="issues-with-removing-an-offboarded-or-decommissioned-device-from-the-device-inventory"></a><span data-ttu-id="7bdb2-102">Problemi sa uklanjanjem rastećeg ili preklonjenog uređaja iz zaliha uređaja</span><span class="sxs-lookup"><span data-stu-id="7bdb2-102">Issues with removing an offboarded or decommissioned device from the Device Inventory</span></span>

<span data-ttu-id="7bdb2-103">Microsoft zaštitnik za krajnju tačku trenutno ne dozvoljava ručno uklanjanje zapisa o uređaju koji je isključen ili je prekid upotrebe uređaja iz zaliha uređaja.</span><span class="sxs-lookup"><span data-stu-id="7bdb2-103">Microsoft Defender for Endpoint does not currently allow manually removing the device record of an offboarded or decommissioned device from the Device Inventory.</span></span>

<span data-ttu-id="7bdb2-104">Iz bezbednosnih razloga uređaj ostaje na portalu kao istorijski zapis do 180 dana.</span><span class="sxs-lookup"><span data-stu-id="7bdb2-104">For security purposes, the device remains in the portal as an historical record for up to 180 days.</span></span> <span data-ttu-id="7bdb2-105">Međutim, podaci o uređaju se prikupljaju u skladu sa konfigurisanim periodom zadržavanja.</span><span class="sxs-lookup"><span data-stu-id="7bdb2-105">However, the device data is purged according to your configured retention period.</span></span>

<span data-ttu-id="7bdb2-106">**Napomogućeno:** Ofboarded or decommissioned device switches automatically to **Inactive state** after seven days.</span><span class="sxs-lookup"><span data-stu-id="7bdb2-106">**Note:** An offboarded or decommissioned device switches automatically to **Inactive** state after seven days.</span></span> <span data-ttu-id="7bdb2-107">Pored toga, uređaji koji nisu aktivni u poslednjih 30 dana ne odražavaju podatke koji odražavaju rezultate izlaganja vaše organizacije Upravljanje pretnjama i ranjivim mestima Microsoft rezultat bezbednosti za uređaje.</span><span class="sxs-lookup"><span data-stu-id="7bdb2-107">In addition, devices not active in the last 30 days are not factored into the data that reflects your organization threat and vulnerability management exposure score or Microsoft Secure Score for Devices.</span></span>
 
<span data-ttu-id="7bdb2-108">Ako i dalje ne želite da vidite određene uređaje u prikazu zaliha uređaja, pokušajte da stavljate oznaku uređaja da biste filtrirali uređaj koji se odvaja iz prikaza zaliha uređaja.</span><span class="sxs-lookup"><span data-stu-id="7bdb2-108">If you still don't want to see certain devices in Device Inventory view, try placing a device tag to filter out the decommissioned device from the Device Inventory view.</span></span>

<span data-ttu-id="7bdb2-109">Za više informacija pogledajte:</span><span class="sxs-lookup"><span data-stu-id="7bdb2-109">For more information, see:</span></span>

[<span data-ttu-id="7bdb2-110">Offboard devices from the Microsoft Defender for Endpoint service</span><span class="sxs-lookup"><span data-stu-id="7bdb2-110">Offboard devices from the Microsoft Defender for Endpoint service</span></span>](/microsoft-365/security/defender-endpoint/offboard-machines.md)

[<span data-ttu-id="7bdb2-111">Rezultat ekspozitora u Upravljanje pretnjama i ranjivim mestima</span><span class="sxs-lookup"><span data-stu-id="7bdb2-111">Exposure score in threat and vulnerability management</span></span>](/microsoft-365/security/defender-endpoint/tvm-exposure-score.md)

[<span data-ttu-id="7bdb2-112">Popravite neisključne senzore u programu Microsoft zaštitnik za krajnje tačke</span><span class="sxs-lookup"><span data-stu-id="7bdb2-112">Fix unhealthy sensors in Microsoft Defender for Endpoint</span></span>](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors#inactive-devices.md)

[<span data-ttu-id="7bdb2-113">Kako se efikasno koristi tagging (1. deo)</span><span class="sxs-lookup"><span data-stu-id="7bdb2-113">How to use tagging effectively (Part 1)</span></span>](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-1/ba-p/1964058)

[<span data-ttu-id="7bdb2-114">Kako se efikasno koristi tagging (2. deo)</span><span class="sxs-lookup"><span data-stu-id="7bdb2-114">How to use tagging effectively (Part 2)</span></span>](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-2/ba-p/1962008)

[<span data-ttu-id="7bdb2-115">Kako se efikasno koristi tagging (3. deo)</span><span class="sxs-lookup"><span data-stu-id="7bdb2-115">How to use tagging effectively (Part 3)</span></span>](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-3/ba-p/1964073)




