---
title: Opcija za otključavanje otiska prsta u operativnom sistemu Windows 10
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
- "9001689"
- "3765"
ms.openlocfilehash: ba1f2e7b0bb54e89178a320b8579b8d1bfdaff9a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/15/2021
ms.locfileid: "51796691"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a><span data-ttu-id="4146e-102">Opcija za otključavanje otiska prsta u operativnom sistemu Windows 10</span><span class="sxs-lookup"><span data-stu-id="4146e-102">Use fingerprint unlock option in Windows 10</span></span>

<span data-ttu-id="4146e-103">**Omogućavanje Windows Hello otiska prsta**</span><span class="sxs-lookup"><span data-stu-id="4146e-103">**Enable Windows Hello Fingerprint**</span></span>

<span data-ttu-id="4146e-104">Da biste otključali Windows 10 pomoću otiska prsta, morate da podesite Windows Hello otisak prsta tako što ćete dodati (što će windows učiti da prepozna) najmanje jednim prstom.</span><span class="sxs-lookup"><span data-stu-id="4146e-104">To unlock Windows 10 using your fingerprint, you need to set up Windows Hello Fingerprint by adding (letting Windows learn to recognize) at least one finger.</span></span> 

1. <span data-ttu-id="4146e-105">Izaberite **stavke Postavke > naloge > za prijavljivanje** (ili kliknite [ovde](ms-settings:signinoptions?activationSource=GetHelp)).</span><span class="sxs-lookup"><span data-stu-id="4146e-105">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="4146e-106">Navodi se dostupne opcije za prijavljivanje.</span><span class="sxs-lookup"><span data-stu-id="4146e-106">Available sign-in options will be listed.</span></span> <span data-ttu-id="4146e-107">Na primer:</span><span class="sxs-lookup"><span data-stu-id="4146e-107">For example:</span></span>

    ![Opcije za prijavljivanje.](media/sign-in-options.png)

2. <span data-ttu-id="4146e-109">Izaberite ili dodirnite **stavku Windows Hello otisak prsta,** a zatim **izaberite stavku Podešavanje**.</span><span class="sxs-lookup"><span data-stu-id="4146e-109">Click or tap **Windows Hello Fingerprint**, then click **Set up**.</span></span> <span data-ttu-id="4146e-110">U prozoru za konfigurisanje usluge Windows Hello kliknite na **dugme Prvi koraci.**</span><span class="sxs-lookup"><span data-stu-id="4146e-110">In the Windows Hello setup window, click **Get started**.</span></span> <span data-ttu-id="4146e-111">Senzor za otisak prsta će se aktivirati i od vas će se tražiti da stavite prst na senzor:</span><span class="sxs-lookup"><span data-stu-id="4146e-111">The fingerprint sensor will activate, and you'll be asked to place your finger on the sensor:</span></span>

   ![Senzor otisaka prstiju.](media/fingerprint-sensor.png)

3. <span data-ttu-id="4146e-113">Sledite uputstva koja će zatražiti od vas da više puta skenirate prst.</span><span class="sxs-lookup"><span data-stu-id="4146e-113">Follow the instructions, which will ask you to repeatedly scan your finger.</span></span> <span data-ttu-id="4146e-114">Kada ovo završite, imaćete opciju da dodate druge prste koje ćete možda želeti da koristite za prijavljivanje.</span><span class="sxs-lookup"><span data-stu-id="4146e-114">When this is finished, you'll have the option of adding other fingers you may want to use for sign-in.</span></span> <span data-ttu-id="4146e-115">Sledeći put kada se prijavite u Windows 10, imaćete opciju da koristite otisak prsta da biste to uraditi.</span><span class="sxs-lookup"><span data-stu-id="4146e-115">Next time you sign in to Windows 10, you will have the option of using your fingerprint to do so.</span></span>

<span data-ttu-id="4146e-116">**Windows Hello otisak prsta nije dostupan kao opcija za prijavljivanje**</span><span class="sxs-lookup"><span data-stu-id="4146e-116">**Windows Hello Fingerprint not available as a sign-in option**</span></span>

<span data-ttu-id="4146e-117">Ako Windows Hello otisak prsta nije prikazan kao opcija u opcijama za **prijavljivanje,** to znači da Windows ne zna za čitač otisaka prstiju/skener povezan sa računarom ili da sistemske smernice sprečavaju njegovu upotrebu (ako na primer, vašim računarom upravlja vaše radno mesto).</span><span class="sxs-lookup"><span data-stu-id="4146e-117">If Windows Hello Fingerprint is not shown as an option in **Sign-in options**, it means Windows is not aware of any fingerprint reader/scanner attached to your PC, or that a system policy prevents its use (if for example your PC is managed by your workplace).</span></span> <span data-ttu-id="4146e-118">Da biste rešili problem:</span><span class="sxs-lookup"><span data-stu-id="4146e-118">To troubleshoot:</span></span> 

1. <span data-ttu-id="4146e-119">Kliknite na **dugme Start** na traci zadataka i potražite stavku **Upravljač uređajima.**</span><span class="sxs-lookup"><span data-stu-id="4146e-119">Select the **Start** button in the Taskbar and search for **Device Manager**.</span></span>

2. <span data-ttu-id="4146e-120">Izaberite ili dodirnite da biste **otvorili Upravljač uređajima.**</span><span class="sxs-lookup"><span data-stu-id="4146e-120">Click or tap to open **Device Manager**.</span></span>

3. <span data-ttu-id="4146e-121">U upravljaču uređajima razvijte biometrijske uređaje tako što ćete kliknuti na ševron.</span><span class="sxs-lookup"><span data-stu-id="4146e-121">In Device Manager, expand Biometric devices by clicking its chevron.</span></span>

   ![Biometrički uređaji.](media/biometric-devices.png)

4. <span data-ttu-id="4146e-123">Skener otisaka prstiju treba da bude naveden kao biometrički uređaj, kao što je Synaptics WBDI skener:</span><span class="sxs-lookup"><span data-stu-id="4146e-123">Your fingerprint scanner should be listed as a biometric device, such as the Synaptics WBDI scanner:</span></span>

   ![Biometrički uređaji.](media/biometric-devices-expanded.png)

5. <span data-ttu-id="4146e-125">Ako skener otisaka prstiju nije prikazan, a skener je integrisan u računar, idite na veb sajt proizvođača računara.</span><span class="sxs-lookup"><span data-stu-id="4146e-125">If your fingerprint scanner is not shown, and the scanner is integrated into your PC, go to the PC manufacturer's website.</span></span> <span data-ttu-id="4146e-126">U odeljku za tehničku podršku za model računara potražite Windows 10 upravljački program za skener koji možete da instalirate.</span><span class="sxs-lookup"><span data-stu-id="4146e-126">In the technical support section for your PC model, search for a Windows 10 driver for a scanner that you can install.</span></span>

6. <span data-ttu-id="4146e-127">Ako je skener odvojen od računara (povezan putem USB),idite na veb sajt proizvođača skenera da biste pronašli i instalirali softver upravljačkog programa Windows 10 uređaja za model skenera koji imate.</span><span class="sxs-lookup"><span data-stu-id="4146e-127">If the scanner is separate from the PC (attached via USB), go to the scanner manufacturer's website to find and install Windows 10 device driver software for the scanner model you have.</span></span>
