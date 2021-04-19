---
title: Ikona napajanja ili baterije nedostaje u operativnom sistemu Windows 10
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002953"
- "5655"
ms.openlocfilehash: 95b68cee58f88d04f02e29477b139f7f583dc0b1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/15/2021
ms.locfileid: "51790562"
---
# <a name="power-or-battery-icon-missing-in-windows-10"></a><span data-ttu-id="7050d-102">Ikona napajanja ili baterije nedostaje u operativnom sistemu Windows 10</span><span class="sxs-lookup"><span data-stu-id="7050d-102">Power or battery icon missing in Windows 10</span></span>

<span data-ttu-id="7050d-103">Ako vaš Windows 10 uređaj ima bateriju (na primer, laptop ili tablet, ili računar povezan putem USB-a sa UPS-om), na primer, na traci zadataka se obično nalazi ikona napajanja/baterije u blizini sata:</span><span class="sxs-lookup"><span data-stu-id="7050d-103">If your Windows 10 device has a battery (e.g., laptop or tablet, or a PC connected via USB to a UPS), normally a power/battery icon is shown in the taskbar near the clock, for example:</span></span>

![Ikona baterije](media/battery-icon.png)

<span data-ttu-id="7050d-105">Ako ne vidite ovu ikonu, možda je skrivena:</span><span class="sxs-lookup"><span data-stu-id="7050d-105">If you don't see this icon, it may be hidden:</span></span>

1. <span data-ttu-id="7050d-106">Idite na **[postavke > Personalizacija > traci zadataka](ms-settings:taskbar?activationSource=GetHelp)**.</span><span class="sxs-lookup"><span data-stu-id="7050d-106">Go to **[Settings > Personalization > Taskbar](ms-settings:taskbar?activationSource=GetHelp)**.</span></span>

2. <span data-ttu-id="7050d-107">Na sistemskoj traci poslova **izaberite stavku Izbor ikona koje će se pojavljivati na traci zadataka.**</span><span class="sxs-lookup"><span data-stu-id="7050d-107">In the Notification area, click **Select which icons appear on the taskbar**.</span></span>

3. <span data-ttu-id="7050d-108">Zatim pronađite **stavku Napajanje** na listi i preklopite njenu postavku na **On**.</span><span class="sxs-lookup"><span data-stu-id="7050d-108">Then find the **Power** item in the list and toggle its setting to **On**.</span></span>

    ![Prikaži ikonu napajanja na traci zadataka](media/power-icon-on.png)

<span data-ttu-id="7050d-110">**Rešavanje problema**</span><span class="sxs-lookup"><span data-stu-id="7050d-110">**Troubleshooting**</span></span>

<span data-ttu-id="7050d-111">Ako ste pratili gorenavedena uputstva i preklopnik napajanja je zasićen ili nije  vidljiv, u polju za pretragu na traci zadataka ukucajte upravljač uređajima **,** a zatim sa liste rezultata izaberite stavku Upravljač uređajima. </span><span class="sxs-lookup"><span data-stu-id="7050d-111">If you followed the above instructions and the **Power** toggle is greyed out or not visible, in the search box on the taskbar, type **device manager**, and then select **Device Manager** in the list of results.</span></span> <span data-ttu-id="7050d-112">U **okviru Baterije kliknite** desnim tasterom miša na bateriju za uređaj, izaberite stavku Onemogući **,** a zatim kliknite na **dugme Da.**</span><span class="sxs-lookup"><span data-stu-id="7050d-112">Under **Batteries**, right-click the battery for your device, click **Disable**, and click **Yes**.</span></span> <span data-ttu-id="7050d-113">Sačekajte nekoliko sekundi, a zatim kliknite desnim tasterom miša na bateriju i izaberite stavku **Omogući.**</span><span class="sxs-lookup"><span data-stu-id="7050d-113">Wait a few seconds, and then right-click the battery and click **Enable**.</span></span> <span data-ttu-id="7050d-114">Zatim ponovo pokrenite uređaj.</span><span class="sxs-lookup"><span data-stu-id="7050d-114">Then restart your device.</span></span>

<span data-ttu-id="7050d-115">Ako ste pratili gorenavedna uputstva, ali se ikona baterije ne pojavljuje na traci zadataka, u polje za pretragu na traci zadataka ukucajte upravljač zadacima **,** a zatim izaberite stavku **Upravljač** zadacima na listi rezultata.</span><span class="sxs-lookup"><span data-stu-id="7050d-115">If you followed the above instructions, but the battery icon does not appear on the taskbar, in the search box on the taskbar, type **task manager**, and then click **Task Manager** in the list of results.</span></span> <span data-ttu-id="7050d-116">Na kartici **Procesi,** u okviru Ime kliknite **desnim tasterom** miša na **Explorer**, a zatim izaberite stavku Ponovo **pokreni.**</span><span class="sxs-lookup"><span data-stu-id="7050d-116">On the **Processes** tab, under **Name**, right-click **Explorer**, and then click **Restart**.</span></span>
