---
title: Korišćenje opcije za otključavanje prsta u operativnom sistemu Windows 10
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
- "9001689"
- "3765"
ms.openlocfilehash: 99f037f62748c06d77b526e35f67b711885c4a1e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/15/2020
ms.locfileid: "47795258"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a><span data-ttu-id="64e1c-102">Korišćenje opcije za otključavanje prsta u operativnom sistemu Windows 10</span><span class="sxs-lookup"><span data-stu-id="64e1c-102">Use fingerprint unlock option in Windows 10</span></span>

<span data-ttu-id="64e1c-103">**Omogućavanje Windows Zdravo otisaka prstiju**</span><span class="sxs-lookup"><span data-stu-id="64e1c-103">**Enable Windows Hello Fingerprint**</span></span>

<span data-ttu-id="64e1c-104">Da biste otključali Windows 10 pomoću otiska prsta, morate da podesite Windows Helo otisak prsta tako što ćete dodati (dopustite da Windows nauči da prepoznaje) bar jedan prst.</span><span class="sxs-lookup"><span data-stu-id="64e1c-104">To unlock Windows 10 using your fingerprint, you need to set up Windows Hello Fingerprint by adding (letting Windows learn to recognize) at least one finger.</span></span> 

1. <span data-ttu-id="64e1c-105">**Izaberite stavke postavke > nalozima > opcijama za prijavljivanje** (ili kliknite [ovde](ms-settings:signinoptions?activationSource=GetHelp)).</span><span class="sxs-lookup"><span data-stu-id="64e1c-105">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="64e1c-106">Dostupne opcije za prijavljivanje će biti navedene.</span><span class="sxs-lookup"><span data-stu-id="64e1c-106">Available sign-in options will be listed.</span></span> <span data-ttu-id="64e1c-107">Na primer:</span><span class="sxs-lookup"><span data-stu-id="64e1c-107">For example:</span></span>

    ![Opcije prijavljivanja.](media/sign-in-options.png)

2. <span data-ttu-id="64e1c-109">Kliknite ili dodirnite stavku **Windows Hello otisak prsta**, a zatim kliknite na dugme **Podesi**.</span><span class="sxs-lookup"><span data-stu-id="64e1c-109">Click or tap **Windows Hello Fingerprint**, then click **Set up**.</span></span> <span data-ttu-id="64e1c-110">U prozoru Podešavanje Windows Helo podešavanje kliknite na dugme **Prvi koraci**.</span><span class="sxs-lookup"><span data-stu-id="64e1c-110">In the Windows Hello setup window, click **Get started**.</span></span> <span data-ttu-id="64e1c-111">Senzor otisaka prstiju će se aktivirati i bićete upitani da postavite prst na senzor:</span><span class="sxs-lookup"><span data-stu-id="64e1c-111">The fingerprint sensor will activate, and you'll be asked to place your finger on the sensor:</span></span>

   ![Senzor otisaka prstiju.](media/fingerprint-sensor.png)

3. <span data-ttu-id="64e1c-113">Izvršite uputstva koja će zatražiti da vam više puta skenira prst.</span><span class="sxs-lookup"><span data-stu-id="64e1c-113">Follow the instructions, which will ask you to repeatedly scan your finger.</span></span> <span data-ttu-id="64e1c-114">Kada se ovo završi, imaćete opciju dodavanja drugih prstiju koje ćete možda želeti da koristite za prijavljivanje.</span><span class="sxs-lookup"><span data-stu-id="64e1c-114">When this is finished, you'll have the option of adding other fingers you may want to use for sign-in.</span></span> <span data-ttu-id="64e1c-115">Sledeći put kada se prijavite u Windows 10, imaćete opciju korišćenja otiska prsta da biste to uradili.</span><span class="sxs-lookup"><span data-stu-id="64e1c-115">Next time you sign in to Windows 10, you will have the option of using your fingerprint to do so.</span></span>

<span data-ttu-id="64e1c-116">**Windows Hello otisak prsta nije dostupan kao opcija za prijavljivanje**</span><span class="sxs-lookup"><span data-stu-id="64e1c-116">**Windows Hello Fingerprint not available as a sign-in option**</span></span>

<span data-ttu-id="64e1c-117">Ako Windows Hello otisak prsta nije prikazan kao opcija u **opcijama za prijavljivanje**, to znači da Windows nije upoznat sa čitačem otisaka prstiju/skenerom priloženim na računaru ili da sistemska smernica sprečava njenu upotrebu (ako na primer, vašem računaru upravlja radno mesto).</span><span class="sxs-lookup"><span data-stu-id="64e1c-117">If Windows Hello Fingerprint is not shown as an option in **Sign-in options**, it means Windows is not aware of any fingerprint reader/scanner attached to your PC, or that a system policy prevents its use (if for example your PC is managed by your workplace).</span></span> <span data-ttu-id="64e1c-118">Da biste rešili problem:</span><span class="sxs-lookup"><span data-stu-id="64e1c-118">To troubleshoot:</span></span> 

1. <span data-ttu-id="64e1c-119">Kliknite na dugme **Start** na traci zadataka i potražite **Upravljač uređajima**.</span><span class="sxs-lookup"><span data-stu-id="64e1c-119">Select the **Start** button in the Taskbar and search for **Device Manager**.</span></span>

2. <span data-ttu-id="64e1c-120">Kliknite ili dodirnite da biste otvorili **Upravljač uređajima**.</span><span class="sxs-lookup"><span data-stu-id="64e1c-120">Click or tap to open **Device Manager**.</span></span>

3. <span data-ttu-id="64e1c-121">U upravljaču uređajima, razvijte biometrijske uređaje tako što ćete kliknuti na njegov simbol.</span><span class="sxs-lookup"><span data-stu-id="64e1c-121">In Device Manager, expand Biometric devices by clicking its chevron.</span></span>

   ![Biometrijski uređaji.](media/biometric-devices.png)

4. <span data-ttu-id="64e1c-123">Skener otisaka prstiju trebalo bi da bude naveden kao biometrijski uređaj, kao što je čitač Sinapetika WBDI:</span><span class="sxs-lookup"><span data-stu-id="64e1c-123">Your fingerprint scanner should be listed as a biometric device, such as the Synaptics WBDI scanner:</span></span>

   ![Biometrijski uređaji.](media/biometric-devices-expanded.png)

5. <span data-ttu-id="64e1c-125">Ako skener za otiske prstiju nije prikazan i ako je skener integrisan u računar, idite na Veb lokaciju proizvođača računara.</span><span class="sxs-lookup"><span data-stu-id="64e1c-125">If your fingerprint scanner is not shown, and the scanner is integrated into your PC, go to the PC manufacturer's website.</span></span> <span data-ttu-id="64e1c-126">U odeljku tehnička podrška za PC model potražite Windows 10 upravljački program za skener koji možete instalirati.</span><span class="sxs-lookup"><span data-stu-id="64e1c-126">In the technical support section for your PC model, search for a Windows 10 driver for a scanner that you can install.</span></span>

6. <span data-ttu-id="64e1c-127">Ako je skener odvojen od računara (priložen pomoću USB-a), idite na Veb lokaciju proizvođača skenera da biste pronašli i instalirali softver za Windows 10 upravljački program za uređaj koji imate.</span><span class="sxs-lookup"><span data-stu-id="64e1c-127">If the scanner is separate from the PC (attached via USB), go to the scanner manufacturer's website to find and install Windows 10 device driver software for the scanner model you have.</span></span>
