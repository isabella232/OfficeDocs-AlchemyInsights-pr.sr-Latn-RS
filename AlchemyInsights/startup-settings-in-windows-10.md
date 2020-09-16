---
title: Postavke pokretanja u operativnom sistemu Windows 10
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
- "9001691"
- "3768"
ms.openlocfilehash: e49faca66785c6611dda702a381c39cdb10884f8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47751149"
---
# <a name="startup-settings-in-windows-10"></a><span data-ttu-id="441f8-102">Postavke pokretanja u operativnom sistemu Windows 10</span><span class="sxs-lookup"><span data-stu-id="441f8-102">Startup settings in Windows 10</span></span>

<span data-ttu-id="441f8-103">**Promena aplikacija automatski se pokreće prilikom pokretanja**</span><span class="sxs-lookup"><span data-stu-id="441f8-103">**Change which apps run automatically at startup**</span></span>

1. <span data-ttu-id="441f8-104">Idite na [postavke > aplikacije > pokretanju](ms-settings:startupapps?activationSource=GetHelp).</span><span class="sxs-lookup"><span data-stu-id="441f8-104">Go to [Settings > Apps > Startup](ms-settings:startupapps?activationSource=GetHelp).</span></span>

2. <span data-ttu-id="441f8-105">Proverite da li **je uključena aplikacija**koju želite da pokrećete prilikom pokretanja.</span><span class="sxs-lookup"><span data-stu-id="441f8-105">Make sure any app you want to run at startup is turned **On**.</span></span>

<span data-ttu-id="441f8-106">**Dodavanje aplikacije za automatsku pokretanje prilikom pokretanja**</span><span class="sxs-lookup"><span data-stu-id="441f8-106">**Add an app to run automatically at startup**</span></span>

1. <span data-ttu-id="441f8-107">Kliknite ili dodirnite stavku **Započni** i pronađite aplikaciju koju želite da pokrenete prilikom pokretanja.</span><span class="sxs-lookup"><span data-stu-id="441f8-107">Click or tap **Start** and find the app you want to run at startup.</span></span>

2. <span data-ttu-id="441f8-108">Kliknite desnim tasterom miša na aplikaciju, kliknite na dugme **još**, a zatim izaberite stavku **Otvori lokaciju datoteke**.</span><span class="sxs-lookup"><span data-stu-id="441f8-108">Right-click the app, click **More**, and then click **Open file location**.</span></span> <span data-ttu-id="441f8-109">Tako ćete otvoriti lokaciju na kojoj se čuva prečica do aplikacije.</span><span class="sxs-lookup"><span data-stu-id="441f8-109">This opens the location where the shortcut to the app is saved.</span></span> <span data-ttu-id="441f8-110">Ako ne postoji opcija za lokaciju za otvaranje datoteke, to znači da aplikacija ne može da se pokrene prilikom pokretanja.</span><span class="sxs-lookup"><span data-stu-id="441f8-110">If there is no option for Open file location, it means the app can't run at startup.</span></span>

3. <span data-ttu-id="441f8-111">Ako je lokacija datoteke otvorena, pritisnite taster sa **Windows logotipom + R**, otkucajte **Shell: pokretanje**, a zatim kliknite na dugme **u redu**.</span><span class="sxs-lookup"><span data-stu-id="441f8-111">With the file location open, press the **Windows logo key  + R**, type **shell:startup**, then click **OK**.</span></span> <span data-ttu-id="441f8-112">Ovo otvara fasciklu za pokretanje.</span><span class="sxs-lookup"><span data-stu-id="441f8-112">This opens the Startup folder.</span></span>

4. <span data-ttu-id="441f8-113">Kopirajte i nalepite prečicu na aplikaciju sa lokacije datoteke u polaznoj fascikli.</span><span class="sxs-lookup"><span data-stu-id="441f8-113">Copy and paste the shortcut to the app from the file location to the Startup folder.</span></span>

<span data-ttu-id="441f8-114">**Napredne opcije pokretanja (uključujući bezbedni režim, UEFI postavke i pokretanje sa drugog uređaja)**</span><span class="sxs-lookup"><span data-stu-id="441f8-114">**Advanced startup options (including Safe Mode, UEFI settings, and booting from another device)**</span></span>

1. <span data-ttu-id="441f8-115">Sačuvajte posao i zatvorite sve otvorene dokumente, pošto će ovi koraci ponovo pokrenuti računar.</span><span class="sxs-lookup"><span data-stu-id="441f8-115">Save your work and close any open documents, since these steps will restart your PC.</span></span>

2. <span data-ttu-id="441f8-116">Idite na [postavke > ažurirajte & bezbednost > oporavku](ms-settings:recovery?activationSource=GetHelp).</span><span class="sxs-lookup"><span data-stu-id="441f8-116">Go to [Settings > Update & Security > Recovery](ms-settings:recovery?activationSource=GetHelp).</span></span>

3. <span data-ttu-id="441f8-117">U okviru **Više opcija za pokretanje**kliknite na dugme **Ponovo pokreni odmah**.</span><span class="sxs-lookup"><span data-stu-id="441f8-117">Under **Advanced startup**, click **Restart now**.</span></span> 

4. <span data-ttu-id="441f8-118">Kada se računar ponovo pokrene na stranici izbor opcije:</span><span class="sxs-lookup"><span data-stu-id="441f8-118">After your PC restarts to the Choose an option screen:</span></span>

    - <span data-ttu-id="441f8-119">Da biste pokrenuli pokretanje sa uređaja kao što je USB disk, kliknite na dugme **koristi uređaj**.</span><span class="sxs-lookup"><span data-stu-id="441f8-119">To boot from a device like a USB drive, click **Use a device**.</span></span>

    - <span data-ttu-id="441f8-120">Da biste uneli postavke UEFI (koje se ponekad nazivaju podešavanje BIOS-a), izaberite stavku **Rešavanje problema > napredne opcije > UEFI firmware postavke**.</span><span class="sxs-lookup"><span data-stu-id="441f8-120">To enter the UEFI settings (sometimes called BIOS setup), click **Troubleshoot > Advanced options > UEFI Firmware Settings**.</span></span> 

    - <span data-ttu-id="441f8-121">Da biste uneli bezbedni režim ili promenili napredne postavke pokretanja, izaberite stavku **rešavanje > više opcija > postavkama pokretanja**, a zatim izaberite stavku **Ponovo pokreni**.</span><span class="sxs-lookup"><span data-stu-id="441f8-121">To enter Safe Mode or change advanced startup settings, click **Troubleshoot > Advanced options > Startup Settings**, then click **Restart**.</span></span> <span data-ttu-id="441f8-122">Od vas će biti zatraženo da unesete [BitLocker ključ za oporavak](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key).</span><span class="sxs-lookup"><span data-stu-id="441f8-122">You may be asked to enter your [BitLocker recovery key](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key).</span></span> <span data-ttu-id="441f8-123">Kada se računar ponovo pokrene, izaberite postavku za pokretanje koju želite da koristite.</span><span class="sxs-lookup"><span data-stu-id="441f8-123">After your PC restarts again, click the startup setting you want to use.</span></span>