---
title: Rešavanje problema sa postojećim monitorom
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
- "3454"
- "9001450"
ms.openlocfilehash: 2dc9a24c1d0d808e26733738cedbc32d513926a0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47690725"
---
# <a name="troubleshoot-an-existing-monitor"></a><span data-ttu-id="812d5-102">Rešavanje problema sa postojećim monitorom</span><span class="sxs-lookup"><span data-stu-id="812d5-102">Troubleshoot an existing monitor</span></span>

<span data-ttu-id="812d5-103">Isprobajte ova rešenja radi rešavanja problema monitoru.</span><span class="sxs-lookup"><span data-stu-id="812d5-103">Try these solutions to troubleshoot a monitor.</span></span> 

<span data-ttu-id="812d5-104">**Osvežite prikaz monitora:**</span><span class="sxs-lookup"><span data-stu-id="812d5-104">**Refresh your monitor's display:**</span></span>

<span data-ttu-id="812d5-105">Istovremeno pritisnite sledeće ključeve: Windows taster + CTRL + SHIFT + B. Ovo će osvežite komunikaciju sa vašim grafičkim upravljačkim programom.</span><span class="sxs-lookup"><span data-stu-id="812d5-105">Press the following keys at the same time: Windows Key  + Ctrl + Shift + B. This will refresh communication with your graphics driver.</span></span> <span data-ttu-id="812d5-106">Monitori će odmah trepnuti i vraćate se poslije nekoliko sekundi.</span><span class="sxs-lookup"><span data-stu-id="812d5-106">Your monitors will blink momentarily and come back after a few seconds.</span></span>

<span data-ttu-id="812d5-107">**Rešavanje problema sa hardverom za monitore:**</span><span class="sxs-lookup"><span data-stu-id="812d5-107">**Troubleshoot monitor hardware:**</span></span>

1. <span data-ttu-id="812d5-108">Isključite kabl koji povezuje računar sa monitorom i ponovo ga priključite.</span><span class="sxs-lookup"><span data-stu-id="812d5-108">Unplug the cable connecting your PC to your monitor, and plug it back in.</span></span>
2. <span data-ttu-id="812d5-109">Isključite sve uređaje koji nisu neophodni sa računara (na primer, adaptere ili pristaniљta).</span><span class="sxs-lookup"><span data-stu-id="812d5-109">Disconnect any non-essential devices from your PC (such as adapters or docks).</span></span>

<span data-ttu-id="812d5-110">**Ako ste nedavno instalirali ispravku na RAČUNARU, možete da vratite upravljački program za prikaz:**</span><span class="sxs-lookup"><span data-stu-id="812d5-110">**If you recently installed an update on your PC, you can roll back your display driver:**</span></span>

1. <span data-ttu-id="812d5-111">Izaberite stavku **Početak**, otkucajte **Upravljač uređajima**i izaberite **Upravljač uređajima** iz rezultata.</span><span class="sxs-lookup"><span data-stu-id="812d5-111">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="812d5-112">Proširite odeljak **adapteri za prikaz** , kliknite desnim tasterom miša na adapter ekrana, a zatim izaberite stavku **Svojstva**.</span><span class="sxs-lookup"><span data-stu-id="812d5-112">Expand the **Display adapters** section, right-click your display adapter, ands select **Properties**.</span></span>
3. <span data-ttu-id="812d5-113">Idite na karticu **upravljački program** i izaberite stavku **Vrati upravljački program**.</span><span class="sxs-lookup"><span data-stu-id="812d5-113">Navigate to the **Driver** tab and select **Roll Back Driver**.</span></span> <br>
<span data-ttu-id="812d5-114">Napomena: ako to nije dostupno ili je sivo, izaberite stavku **ne** iz dolenavedenih opcija da biste prešli na sledeći korak.</span><span class="sxs-lookup"><span data-stu-id="812d5-114">Note: If this isn't available or is grayed out, select **No** from the options below to move to the next step.</span></span>
4. <span data-ttu-id="812d5-115">Možda ćete morati ponovo da pokrenete računar da bi ove promene stupile na snagu.</span><span class="sxs-lookup"><span data-stu-id="812d5-115">You may need to restart your PC before these changes take effect.</span></span>

<span data-ttu-id="812d5-116">**Deinstalirajte i ponovo instalirajte upravljački program za prikaz:**</span><span class="sxs-lookup"><span data-stu-id="812d5-116">**Uninstall and reinstall your display driver:**</span></span>

1. <span data-ttu-id="812d5-117">Izaberite stavku **Početak**, otkucajte **Upravljač uređajima**i izaberite **Upravljač uređajima** iz rezultata.</span><span class="sxs-lookup"><span data-stu-id="812d5-117">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="812d5-118">Razvijte odeljak **adapteri za prikaz** , kliknite desnim tasterom miša na adapter ekrana, ands izaberite stavku **Deinstaliraj uređaj**.</span><span class="sxs-lookup"><span data-stu-id="812d5-118">Expand the **Display adapters** section, right-click your display adapter, ands select **Uninstall device**.</span></span> 
3. <span data-ttu-id="812d5-119">Potvrdite izbor u polju za potvrdu pored opcije **Izbriši softver upravljačkog programa za ovaj uređaj** i izaberite stavku **Deinstaliraj**.</span><span class="sxs-lookup"><span data-stu-id="812d5-119">Select the box next to **Delete the driver software for this device** and select **Uninstall**.</span></span><br>
<span data-ttu-id="812d5-120">Napomena: možda će vam biti zatraženo da ponovo pokrenete računar u ovoj fazi.</span><span class="sxs-lookup"><span data-stu-id="812d5-120">Note: You may be asked to restart your computer at this stage.</span></span> <span data-ttu-id="812d5-121">Obavezno zapišite preostale instrukcije pre nego što ponovo pokrenete.</span><span class="sxs-lookup"><span data-stu-id="812d5-121">Make sure to write down the remaining instructions before you restart.</span></span>
4. <span data-ttu-id="812d5-122">Ponovo otvorite Upravljač uređajima.</span><span class="sxs-lookup"><span data-stu-id="812d5-122">Open Device Manager again.</span></span>
5. <span data-ttu-id="812d5-123">Proširite odeljak **adapteri za prikaz** , kliknite desnim tasterom miša na adapter ekrana i izaberite stavku **Ažuriraj upravljački program**.</span><span class="sxs-lookup"><span data-stu-id="812d5-123">Expand the **Display adapters** section, right-click on your display adapter, and select **Update Driver**.</span></span>
6. <span data-ttu-id="812d5-124">Izaberite stavku **Pretraži automatski za ažuriranje softvera upravljačkog programa** i kliknite na uputstvo za instalaciju.</span><span class="sxs-lookup"><span data-stu-id="812d5-124">Select **Search automatically for update driver software** and follow the installation instructions.</span></span>