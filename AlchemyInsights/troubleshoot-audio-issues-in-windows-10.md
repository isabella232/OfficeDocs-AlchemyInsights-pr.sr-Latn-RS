---
title: Rešavanje problema sa zvukom u operativnom sistemu Windows 10
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
- "3476"
- "9001463"
ms.openlocfilehash: 88157f9c82bc970e989d47f5cf376b7ce485cb2a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47750357"
---
# <a name="troubleshooting-audio-issues-in-windows-10"></a><span data-ttu-id="3e480-102">Rešavanje problema sa zvukom u operativnom sistemu Windows 10</span><span class="sxs-lookup"><span data-stu-id="3e480-102">Troubleshooting audio issues in Windows 10</span></span>

<span data-ttu-id="3e480-103">**Pokrenite alatku za rešavanje problema sa zvukom**</span><span class="sxs-lookup"><span data-stu-id="3e480-103">**Run the audio troubleshooter**</span></span>

1.  <span data-ttu-id="3e480-104">Otvorite [Postavke rešavanja problema](ms-settings:troubleshoot).</span><span class="sxs-lookup"><span data-stu-id="3e480-104">Open the [Troubleshoot settings](ms-settings:troubleshoot).</span></span>

2.  <span data-ttu-id="3e480-105">Izaberite stavku **reprodukovanje zvuka**  >  **pokrenite alatku za rešavanje problema**.</span><span class="sxs-lookup"><span data-stu-id="3e480-105">Select **Playing Audio** > **Run the troubleshooter**.</span></span>

<span data-ttu-id="3e480-106">**Postavljanje podrazumevanog uređaja**</span><span class="sxs-lookup"><span data-stu-id="3e480-106">**Set the default device**</span></span>

<span data-ttu-id="3e480-107">Ako se povezujete sa audio uređajem koristeći USB ili HDMI, možda ćete morati da ga konfigurišete kao podrazumevanog:</span><span class="sxs-lookup"><span data-stu-id="3e480-107">If you're connecting to an audio device using USB or HDMI, you might need to set that device as the default:</span></span>

1. <span data-ttu-id="3e480-108">Otvorite **početni**  >  **zvuk**, a zatim izaberite stavku **zvuk zvuka** ili **promenite zvukove sistema** sa liste rezultata.</span><span class="sxs-lookup"><span data-stu-id="3e480-108">Open **Start** > **Sound**, and then select **Sound** or **Change system sounds** from the list of results.</span></span>

2.  <span data-ttu-id="3e480-109">Na kartici **Reprodukcija** izaberite uređaj, izaberite stavku **Postavi podrazumevano**, a zatim kliknite na **dugme u redu**.</span><span class="sxs-lookup"><span data-stu-id="3e480-109">On the **Playback** tab, select a device, select **Set Default**, and then select **OK**.</span></span>

<span data-ttu-id="3e480-110">**Proveravanje kablova, volumena, zvučnika i slušalica**</span><span class="sxs-lookup"><span data-stu-id="3e480-110">**Check cables, volume, speakers, and headphones**</span></span>

1. <span data-ttu-id="3e480-111">Proverite veze govornika i slušalice za labavu kablove i uverite se da su povezani sa ispravnim konektorom.</span><span class="sxs-lookup"><span data-stu-id="3e480-111">Check your speaker and headphone connections for loose cables, and make sure they're connected to the correct jack.</span></span>

2. <span data-ttu-id="3e480-112">Potvrdite izbor u polju za funkciju Power i volumen i Isprobajte sve kontrole volumena.</span><span class="sxs-lookup"><span data-stu-id="3e480-112">Check your power and volume levels and try turning all the volume controls up.</span></span>

3. <span data-ttu-id="3e480-113">Neki zvučnici i aplikacije imaju sopstvene kontrole volumena; Možda ćete morati da ih proverite da biste se uverili da su na pravom nivou.</span><span class="sxs-lookup"><span data-stu-id="3e480-113">Some speakers and apps have their own volume controls; you might have to check them all to make sure they're at the right levels.</span></span>

4. <span data-ttu-id="3e480-114">Pokušajte da se povežete pomoću drugog USB porta.</span><span class="sxs-lookup"><span data-stu-id="3e480-114">Try connecting using a different USB port.</span></span>

<span data-ttu-id="3e480-115">**Napomena**: Imajte na umu da zvučnici možda neće raditi kada su slušalice priključeni.</span><span class="sxs-lookup"><span data-stu-id="3e480-115">**Note**: Remember that your speakers may not work when headphones are plugged in.</span></span>

<span data-ttu-id="3e480-116">**Proveravanje upravljača uređajima**</span><span class="sxs-lookup"><span data-stu-id="3e480-116">**Check Device Manager**</span></span>

<span data-ttu-id="3e480-117">Da biste se uverili da su upravljački programi ažurni:</span><span class="sxs-lookup"><span data-stu-id="3e480-117">To make sure the drivers are up to date:</span></span>

1. <span data-ttu-id="3e480-118">Izaberite stavku **Start**, otkucajte **Upravljač uređajima**, a zatim izaberite **Upravljač uređajima** sa liste rezultata.</span><span class="sxs-lookup"><span data-stu-id="3e480-118">Select **Start**, type **Device Manager**, and then select **Device Manager** from the list of results.</span></span>

2. <span data-ttu-id="3e480-119">U okviru Excel **, video i upravljači za igre**izaberite zvučnu karticu, otvorite je, izaberite karticu **upravljački program** i izaberite stavku **Ažuriraj upravljački program**.</span><span class="sxs-lookup"><span data-stu-id="3e480-119">Under **Sound, video, and game controllers**, select your sound card, open it, select the **Driver** tab, and select **Update Driver**.</span></span>

<span data-ttu-id="3e480-120">**Napomena**: Ako Windows ne pronađe novi upravljački program, potražite ga na Veb lokaciji proizvođača uređaja i slede uputstva.</span><span class="sxs-lookup"><span data-stu-id="3e480-120">**Note**: If Windows doesn't find a new driver, look for one on the device manufacturer's website and follow their instructions.</span></span>

<span data-ttu-id="3e480-121">**Ponovno instaliranje upravljačkog programa**</span><span class="sxs-lookup"><span data-stu-id="3e480-121">**Reinstall the driver**</span></span>

<span data-ttu-id="3e480-122">Ako ne možete da ažurirate pomoću upravljača uređajima ili pronađete novi upravljački program na Veb lokaciji proizvođača, isprobajte ove korake:</span><span class="sxs-lookup"><span data-stu-id="3e480-122">If you can't update via Device Manager or find a new driver on the manufacturer's website, try these steps:</span></span>

1. <span data-ttu-id="3e480-123">U upravljaču uređajima kliknite desnim tasterom miša (ili pritisnite i držite) audio upravljački program i izaberite stavku **Deinstaliraj**.</span><span class="sxs-lookup"><span data-stu-id="3e480-123">In Device Manager, right-click (or press and hold) the audio driver, and select **Uninstall**.</span></span> <span data-ttu-id="3e480-124">Ponovo pokrenite uređaj i Windows će pokušati da ponovo instalira upravljački program.</span><span class="sxs-lookup"><span data-stu-id="3e480-124">Restart your device and Windows will attempt to reinstall the driver.</span></span>

2. <span data-ttu-id="3e480-125">Ako ponovna instalacija upravljačkog programa ne radi, pokušajte da koristite generički audio upravljački program koji se dobija uz Windows.</span><span class="sxs-lookup"><span data-stu-id="3e480-125">If reinstalling the driver doesn't work, try using the generic audio driver that comes with Windows.</span></span> <span data-ttu-id="3e480-126">U upravljaču uređajima, kliknite desnim tasterom miša na stavku (ili ga pritisnite i zadržite) > upravljački program za **Ažuriranje softvera za upravljačke**programe  >  **Pregledajte računar za softver upravljačkog programa**  >  **Dozvoli mi da izaberem sa liste upravljačkih programa uređaja na računaru**, izaberite stavku **audio uređaj visoke definicije**, izaberite stavku **dalje**i praćenje uputstava za instaliranje.</span><span class="sxs-lookup"><span data-stu-id="3e480-126">In Device Manager, right-click (or press and hold) your audio driver > **Update driver software** > **Browse my computer for driver software** > **Let me pick from a list of device drivers on my computer**, select **High Definition Audio Device**, select **Next**, and follow the instructions to install it.</span></span>
