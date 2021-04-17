---
title: Rešavanje problema sa postojećim monitorom
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
- "3454"
- "9001450"
ms.openlocfilehash: c4d2bb64b6b5ea79d4cd585e2be85c3c17e0f76f
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/15/2021
ms.locfileid: "51824593"
---
# <a name="troubleshoot-an-existing-monitor"></a><span data-ttu-id="696b3-102">Rešavanje problema sa postojećim monitorom</span><span class="sxs-lookup"><span data-stu-id="696b3-102">Troubleshoot an existing monitor</span></span>

<span data-ttu-id="696b3-103">Isprobajte ova rešenja za rešavanje problema sa monitorom.</span><span class="sxs-lookup"><span data-stu-id="696b3-103">Try these solutions to troubleshoot a monitor.</span></span> 

<span data-ttu-id="696b3-104">**Osvežite prikaz monitora:**</span><span class="sxs-lookup"><span data-stu-id="696b3-104">**Refresh your monitor's display:**</span></span>

<span data-ttu-id="696b3-105">Istovremeno pritisnite sledeće tastere: Windows taster + Ctrl + Shift + B. To će osvežiti komunikaciju sa vašim upravljačkim programom grafičke grafike.</span><span class="sxs-lookup"><span data-stu-id="696b3-105">Press the following keys at the same time: Windows Key  + Ctrl + Shift + B. This will refresh communication with your graphics driver.</span></span> <span data-ttu-id="696b3-106">Monitori će trenutno treperiti i vratiti se posle nekoliko sekundi.</span><span class="sxs-lookup"><span data-stu-id="696b3-106">Your monitors will blink momentarily and come back after a few seconds.</span></span>

<span data-ttu-id="696b3-107">**Rešavanje problema sa hardverom monitora:**</span><span class="sxs-lookup"><span data-stu-id="696b3-107">**Troubleshoot monitor hardware:**</span></span>

1. <span data-ttu-id="696b3-108">Isključite kabl koji povezuje računar sa monitorom i ponovo ga priključite.</span><span class="sxs-lookup"><span data-stu-id="696b3-108">Unplug the cable connecting your PC to your monitor, and plug it back in.</span></span>
2. <span data-ttu-id="696b3-109">Prekinite vezu sa računarom koji nije nevažni uređaj (kao što su adapteri ili dock-na).</span><span class="sxs-lookup"><span data-stu-id="696b3-109">Disconnect any non-essential devices from your PC (such as adapters or docks).</span></span>

<span data-ttu-id="696b3-110">**Ako ste nedavno instalirali ispravku na računaru, možete da vratite upravljački program ekrana:**</span><span class="sxs-lookup"><span data-stu-id="696b3-110">**If you recently installed an update on your PC, you can roll back your display driver:**</span></span>

1. <span data-ttu-id="696b3-111">Izaberite **start**, **otkucajte upravljač uređajima** i u **rezultatima izaberite** stavku Upravljač uređajima.</span><span class="sxs-lookup"><span data-stu-id="696b3-111">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="696b3-112">Razvijte odeljak **Video adapteri,** kliknite desnim tasterom miša na video adapter i izaberite stavku **Svojstva.**</span><span class="sxs-lookup"><span data-stu-id="696b3-112">Expand the **Display adapters** section, right-click your display adapter, ands select **Properties**.</span></span>
3. <span data-ttu-id="696b3-113">Prešli na karticu Upravljački program **i izaberite** stavku Vrati **upravljački program .**</span><span class="sxs-lookup"><span data-stu-id="696b3-113">Navigate to the **Driver** tab and select **Roll Back Driver**.</span></span> <br>
<span data-ttu-id="696b3-114">Napomiće: Ako to nije dostupno  ili je zasivo, izaberite ne u opcijama u nastavku da biste prešli na sledeći korak.</span><span class="sxs-lookup"><span data-stu-id="696b3-114">Note: If this isn't available or is grayed out, select **No** from the options below to move to the next step.</span></span>
4. <span data-ttu-id="696b3-115">Možda ćete morati ponovo da pokrenete računar pre nego što ove promene stupiju na snagu.</span><span class="sxs-lookup"><span data-stu-id="696b3-115">You may need to restart your PC before these changes take effect.</span></span>

<span data-ttu-id="696b3-116">**Deinstalujte i ponovo instalirajte upravljački program za prikaz:**</span><span class="sxs-lookup"><span data-stu-id="696b3-116">**Uninstall and reinstall your display driver:**</span></span>

1. <span data-ttu-id="696b3-117">Izaberite **start**, **otkucajte upravljač uređajima** i u **rezultatima izaberite** stavku Upravljač uređajima.</span><span class="sxs-lookup"><span data-stu-id="696b3-117">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="696b3-118">Razvijte **odeljak Video adapteri,** kliknite desnim tasterom miša na video adapter i izaberite **stavku Deinstaliranje uređaja**.</span><span class="sxs-lookup"><span data-stu-id="696b3-118">Expand the **Display adapters** section, right-click your display adapter, ands select **Uninstall device**.</span></span> 
3. <span data-ttu-id="696b3-119">Potvrdite izbor u polju za potvrdu **pored stavke Izbriši softver upravljačkog programa za ovaj uređaj** i **izaberite stavku Deinstaliranje**.</span><span class="sxs-lookup"><span data-stu-id="696b3-119">Select the box next to **Delete the driver software for this device** and select **Uninstall**.</span></span><br>
<span data-ttu-id="696b3-120">Napomi: Od vas se može tražiti da u ovoj fazi ponovo pokrenete računar.</span><span class="sxs-lookup"><span data-stu-id="696b3-120">Note: You may be asked to restart your computer at this stage.</span></span> <span data-ttu-id="696b3-121">Zapišite preostala uputstva pre ponovnog pokretanja.</span><span class="sxs-lookup"><span data-stu-id="696b3-121">Make sure to write down the remaining instructions before you restart.</span></span>
4. <span data-ttu-id="696b3-122">Ponovo otvorite upravljač uređajima.</span><span class="sxs-lookup"><span data-stu-id="696b3-122">Open Device Manager again.</span></span>
5. <span data-ttu-id="696b3-123">Razvijte odeljak **Video adapteri,** kliknite desnim tasterom miša na video adapter i izaberite stavku Ažuriraj upravljački **program.**</span><span class="sxs-lookup"><span data-stu-id="696b3-123">Expand the **Display adapters** section, right-click on your display adapter, and select **Update Driver**.</span></span>
6. <span data-ttu-id="696b3-124">Izaberite **stavku Automatski pretraži za ažuriranje softvera upravljačkog programa** i pratite uputstva za instaliranje.</span><span class="sxs-lookup"><span data-stu-id="696b3-124">Select **Search automatically for update driver software** and follow the installation instructions.</span></span>