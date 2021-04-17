---
title: Rešavanje problema sa zvukom u operativnom sistemu Windows 10
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
- "3476"
- "9001463"
ms.openlocfilehash: 1bafc97b2ab1394087d2451d73168a29267d64ab
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833305"
---
# <a name="troubleshooting-audio-issues-in-windows-10"></a><span data-ttu-id="783fa-102">Rešavanje problema sa zvukom u operativnom sistemu Windows 10</span><span class="sxs-lookup"><span data-stu-id="783fa-102">Troubleshooting audio issues in Windows 10</span></span>

<span data-ttu-id="783fa-103">**Pokretanje alatke za rešavanje problema sa zvukom**</span><span class="sxs-lookup"><span data-stu-id="783fa-103">**Run the audio troubleshooter**</span></span>

1.  <span data-ttu-id="783fa-104">Otvorite postavke [Rešavanje problema](ms-settings:troubleshoot).</span><span class="sxs-lookup"><span data-stu-id="783fa-104">Open the [Troubleshoot settings](ms-settings:troubleshoot).</span></span>

2.  <span data-ttu-id="783fa-105">Izaberite **reprodukuj zvuk**  >  **Pokreni alatku za rešavanje problema**.</span><span class="sxs-lookup"><span data-stu-id="783fa-105">Select **Playing Audio** > **Run the troubleshooter**.</span></span>

<span data-ttu-id="783fa-106">**Podešavanje podrazumevanog uređaja**</span><span class="sxs-lookup"><span data-stu-id="783fa-106">**Set the default device**</span></span>

<span data-ttu-id="783fa-107">Ako se povezujete sa audio uređajem pomoću USB ili HDMI veze, možda ćete morati da podesite taj uređaj kao podrazumevani:</span><span class="sxs-lookup"><span data-stu-id="783fa-107">If you're connecting to an audio device using USB or HDMI, you might need to set that device as the default:</span></span>

1. <span data-ttu-id="783fa-108">U **listi rezultata** izaberite stavku Pokreni zvuk, a  >  zatim izaberite stavku Zvuk ili Promena sistemskih zvukova.  </span><span class="sxs-lookup"><span data-stu-id="783fa-108">Open **Start** > **Sound**, and then select **Sound** or **Change system sounds** from the list of results.</span></span>

2.  <span data-ttu-id="783fa-109">Na kartici **Reprodukcija izaberite** uređaj, izaberite stavku Postavi **podrazumevano**, a zatim kliknite na dugme **U redu.**</span><span class="sxs-lookup"><span data-stu-id="783fa-109">On the **Playback** tab, select a device, select **Set Default**, and then select **OK**.</span></span>

<span data-ttu-id="783fa-110">**Proverite kablove, jačinu zvuka, zvučnike i slušalice**</span><span class="sxs-lookup"><span data-stu-id="783fa-110">**Check cables, volume, speakers, and headphones**</span></span>

1. <span data-ttu-id="783fa-111">Proverite da li kablovi zvučnika i slušalica nisu priključeni kablovi i proverite da li su povezani sa odgovarajućim konektorom.</span><span class="sxs-lookup"><span data-stu-id="783fa-111">Check your speaker and headphone connections for loose cables, and make sure they're connected to the correct jack.</span></span>

2. <span data-ttu-id="783fa-112">Proverite nivo napajanja i jačine zvuka i pokušajte da povećate jačinu zvuka.</span><span class="sxs-lookup"><span data-stu-id="783fa-112">Check your power and volume levels and try turning all the volume controls up.</span></span>

3. <span data-ttu-id="783fa-113">Neki zvučnici i aplikacije imaju sopstvene kontrole zvuka; možda ćete morati da ih sve proverite da biste se uverili da su na pravom nivou.</span><span class="sxs-lookup"><span data-stu-id="783fa-113">Some speakers and apps have their own volume controls; you might have to check them all to make sure they're at the right levels.</span></span>

4. <span data-ttu-id="783fa-114">Pokušajte da se povežete koristeći drugi USB port.</span><span class="sxs-lookup"><span data-stu-id="783fa-114">Try connecting using a different USB port.</span></span>

<span data-ttu-id="783fa-115">**Naznaka:** Ne zaboravite da zvučnici možda neće raditi kada su slušalice priključene.</span><span class="sxs-lookup"><span data-stu-id="783fa-115">**Note**: Remember that your speakers may not work when headphones are plugged in.</span></span>

<span data-ttu-id="783fa-116">**Provera u upravljaču uređajima**</span><span class="sxs-lookup"><span data-stu-id="783fa-116">**Check Device Manager**</span></span>

<span data-ttu-id="783fa-117">Da biste se uverili da su upravljački programi aženjeni:</span><span class="sxs-lookup"><span data-stu-id="783fa-117">To make sure the drivers are up to date:</span></span>

1. <span data-ttu-id="783fa-118">Izaberite **start**, **otkucajte Upravljač uređajima**, a zatim **sa** liste rezultata izaberite stavku Upravljač uređajima.</span><span class="sxs-lookup"><span data-stu-id="783fa-118">Select **Start**, type **Device Manager**, and then select **Device Manager** from the list of results.</span></span>

2. <span data-ttu-id="783fa-119">U **okviru Upravljači zvukom, videom** i igrom  izaberite zvučnu karticu, otvorite je, izaberite karticu Upravljački program i izaberite stavku **Ažuriraj** upravljački program .</span><span class="sxs-lookup"><span data-stu-id="783fa-119">Under **Sound, video, and game controllers**, select your sound card, open it, select the **Driver** tab, and select **Update Driver**.</span></span>

<span data-ttu-id="783fa-120">**Napomi:** Ako Windows ne pronađe novi upravljački program, pronađite ga na veb lokaciji proizvođača uređaja i pratite njihova uputstva.</span><span class="sxs-lookup"><span data-stu-id="783fa-120">**Note**: If Windows doesn't find a new driver, look for one on the device manufacturer's website and follow their instructions.</span></span>

<span data-ttu-id="783fa-121">**Ponovo instalirajte upravljački program**</span><span class="sxs-lookup"><span data-stu-id="783fa-121">**Reinstall the driver**</span></span>

<span data-ttu-id="783fa-122">Ako ne možete da ažurirate putem upravljača uređajima ili pronađete novi upravljački program na veb lokaciji proizvođača, isprobajte ove korake:</span><span class="sxs-lookup"><span data-stu-id="783fa-122">If you can't update via Device Manager or find a new driver on the manufacturer's website, try these steps:</span></span>

1. <span data-ttu-id="783fa-123">U upravljaču uređajima kliknite desnim tasterom miša na (ili pritisnite i držite) upravljački program za zvuk i izaberite **stavku Deinstaliranje**.</span><span class="sxs-lookup"><span data-stu-id="783fa-123">In Device Manager, right-click (or press and hold) the audio driver, and select **Uninstall**.</span></span> <span data-ttu-id="783fa-124">Ponovo pokrenite uređaj i Windows će pokušati da ponovo instalira upravljački program.</span><span class="sxs-lookup"><span data-stu-id="783fa-124">Restart your device and Windows will attempt to reinstall the driver.</span></span>

2. <span data-ttu-id="783fa-125">Ako poništavanje instalacije upravljačkog programa ne funkcioniše, pokušajte da koristite generički upravljački program za zvuk koji se dolazi uz Windows.</span><span class="sxs-lookup"><span data-stu-id="783fa-125">If reinstalling the driver doesn't work, try using the generic audio driver that comes with Windows.</span></span> <span data-ttu-id="783fa-126">U upravljaču uređajima kliknite desnim tasterom miša na upravljački program za zvuk (ili ga pritisnite i držite) > Ažuriraj softver upravljačkog programa Potraži softver upravljačkog programa Na računaru pronađi softver upravljačkog programa Dozvolite mi da izaberem sa liste upravljačkih programa uređaja na računaru, izaberite stavku Audio uređaj  >  **visoke definicije,** kliknite na dugme Dalje i pratite uputstva da biste ga  >  instalirali.  </span><span class="sxs-lookup"><span data-stu-id="783fa-126">In Device Manager, right-click (or press and hold) your audio driver > **Update driver software** > **Browse my computer for driver software** > **Let me pick from a list of device drivers on my computer**, select **High Definition Audio Device**, select **Next**, and follow the instructions to install it.</span></span>
