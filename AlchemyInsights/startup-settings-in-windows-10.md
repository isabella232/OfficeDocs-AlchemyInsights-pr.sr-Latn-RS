---
title: Postavke pokretanja u operativnom sistemu Windows 10
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
- "9001691"
- "3768"
ms.openlocfilehash: 6dfae58a398db088ba00d9c2ea9788bab929ccc1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/15/2021
ms.locfileid: "51828166"
---
# <a name="startup-settings-in-windows-10"></a><span data-ttu-id="6df20-102">Postavke pokretanja u operativnom sistemu Windows 10</span><span class="sxs-lookup"><span data-stu-id="6df20-102">Startup settings in Windows 10</span></span>

<span data-ttu-id="6df20-103">**Promena aplikacija koje se pokrećaju automatski pri pokretanju**</span><span class="sxs-lookup"><span data-stu-id="6df20-103">**Change which apps run automatically at startup**</span></span>

1. <span data-ttu-id="6df20-104">Idite na [Postavke > Aplikacije > pokretanje](ms-settings:startupapps?activationSource=GetHelp).</span><span class="sxs-lookup"><span data-stu-id="6df20-104">Go to [Settings > Apps > Startup](ms-settings:startupapps?activationSource=GetHelp).</span></span>

2. <span data-ttu-id="6df20-105">Uverite se da je uključena bilo koja aplikacija koju želite da pokrenete pri **pokretanju.**</span><span class="sxs-lookup"><span data-stu-id="6df20-105">Make sure any app you want to run at startup is turned **On**.</span></span>

<span data-ttu-id="6df20-106">**Dodavanje aplikacije koja će se automatski pokrenuti pri pokretanju**</span><span class="sxs-lookup"><span data-stu-id="6df20-106">**Add an app to run automatically at startup**</span></span>

1. <span data-ttu-id="6df20-107">Kliknite na dugme **Start ili je** dodirnite i pronađite aplikaciju koju želite da pokrenete pri pokretanju.</span><span class="sxs-lookup"><span data-stu-id="6df20-107">Click or tap **Start** and find the app you want to run at startup.</span></span>

2. <span data-ttu-id="6df20-108">Kliknite desnim tasterom miša na aplikaciju, izaberite **stavku Još**, a zatim **izaberite stavku Otvori lokaciju datoteke**.</span><span class="sxs-lookup"><span data-stu-id="6df20-108">Right-click the app, click **More**, and then click **Open file location**.</span></span> <span data-ttu-id="6df20-109">To otvara lokaciju na kojoj je sačuvana prečica do aplikacije.</span><span class="sxs-lookup"><span data-stu-id="6df20-109">This opens the location where the shortcut to the app is saved.</span></span> <span data-ttu-id="6df20-110">Ako ne postoji opcija za Otvaranje lokacije datoteke, to znači da aplikacija ne može da se pokrene pri pokretanju.</span><span class="sxs-lookup"><span data-stu-id="6df20-110">If there is no option for Open file location, it means the app can't run at startup.</span></span>

3. <span data-ttu-id="6df20-111">Kada je lokacija datoteke otvorena, pritisnite taster sa **Windows logotipom + R**, otkucajte **shell:startup**, a zatim kliknite na dugme **U redu**.</span><span class="sxs-lookup"><span data-stu-id="6df20-111">With the file location open, press the **Windows logo key  + R**, type **shell:startup**, then click **OK**.</span></span> <span data-ttu-id="6df20-112">To otvara fasciklu "Pokretanje".</span><span class="sxs-lookup"><span data-stu-id="6df20-112">This opens the Startup folder.</span></span>

4. <span data-ttu-id="6df20-113">Kopirajte i nalepite prečicu do aplikacije sa lokacije datoteke u pokrenu fasciklu.</span><span class="sxs-lookup"><span data-stu-id="6df20-113">Copy and paste the shortcut to the app from the file location to the Startup folder.</span></span>

<span data-ttu-id="6df20-114">**Napredne opcije za pokretanje (uključujući bezbedni režim, UEFI postavke i pokretanje sa drugog uređaja)**</span><span class="sxs-lookup"><span data-stu-id="6df20-114">**Advanced startup options (including Safe Mode, UEFI settings, and booting from another device)**</span></span>

1. <span data-ttu-id="6df20-115">Sačuvajte rad i zatvorite sve otvorene dokumente jer će ovi koraci ponovo pokrenuti računar.</span><span class="sxs-lookup"><span data-stu-id="6df20-115">Save your work and close any open documents, since these steps will restart your PC.</span></span>

2. <span data-ttu-id="6df20-116">Idite na [Postavke > Ažuriranje & bezbednosti > oporavak.](ms-settings:recovery?activationSource=GetHelp)</span><span class="sxs-lookup"><span data-stu-id="6df20-116">Go to [Settings > Update & Security > Recovery](ms-settings:recovery?activationSource=GetHelp).</span></span>

3. <span data-ttu-id="6df20-117">U **okviru Napredno pokretanje izaberite** stavku **Ponovo pokreni odmah.**</span><span class="sxs-lookup"><span data-stu-id="6df20-117">Under **Advanced startup**, click **Restart now**.</span></span> 

4. <span data-ttu-id="6df20-118">Kada se računar ponovo pokrene na ekran Izbor opcije:</span><span class="sxs-lookup"><span data-stu-id="6df20-118">After your PC restarts to the Choose an option screen:</span></span>

    - <span data-ttu-id="6df20-119">Da biste se pokrećeli sa uređaja kao što je USB disk, **izaberite stavku Koristi uređaj**.</span><span class="sxs-lookup"><span data-stu-id="6df20-119">To boot from a device like a USB drive, click **Use a device**.</span></span>

    - <span data-ttu-id="6df20-120">Da biste uneli UEFI postavke (ponekad se naziva BIOS podešavanje), izaberite stavku Rešavanje problema > napredne opcije **> UEFI postavke firmvera.**</span><span class="sxs-lookup"><span data-stu-id="6df20-120">To enter the UEFI settings (sometimes called BIOS setup), click **Troubleshoot > Advanced options > UEFI Firmware Settings**.</span></span> 

    - <span data-ttu-id="6df20-121">Da biste ušli u bezbedni režim ili promenili postavke naprednog pokretanja, izaberite stavku **Rešavanje problema > napredne** opcije i > postavki pokretanja, a zatim izaberite stavku **Ponovo pokreni.**</span><span class="sxs-lookup"><span data-stu-id="6df20-121">To enter Safe Mode or change advanced startup settings, click **Troubleshoot > Advanced options > Startup Settings**, then click **Restart**.</span></span> <span data-ttu-id="6df20-122">Možda će vam biti zatraženo da [unesete BitLocker ključ za oporavak.](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key)</span><span class="sxs-lookup"><span data-stu-id="6df20-122">You may be asked to enter your [BitLocker recovery key](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key).</span></span> <span data-ttu-id="6df20-123">Kada se računar ponovo pokrene, kliknite na postavku pokretanja koji želite da koristite.</span><span class="sxs-lookup"><span data-stu-id="6df20-123">After your PC restarts again, click the startup setting you want to use.</span></span>