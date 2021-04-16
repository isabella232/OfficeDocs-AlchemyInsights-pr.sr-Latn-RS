---
title: Rešavanje problema sa Bluetooth omogom u operativnom sistemu Windows 10
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
- "9001475"
- "3506"
ms.openlocfilehash: f20bf4a642e019c7901e988a027e0220f0f1b07b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/15/2021
ms.locfileid: "51812946"
---
# <a name="fix-bluetooth-problems-in-windows-10"></a><span data-ttu-id="ac2cf-102">Rešavanje problema sa Bluetooth omogom u operativnom sistemu Windows 10</span><span class="sxs-lookup"><span data-stu-id="ac2cf-102">Fix Bluetooth problems in Windows 10</span></span>

<span data-ttu-id="ac2cf-103">Ako ikona za Bluetooth nedostaje ili Bluetooth ne može da se uključi ili isključi, trebalo bi da pokrenete alatku za rešavanje problema sa Bluetooth omogom.</span><span class="sxs-lookup"><span data-stu-id="ac2cf-103">If the Bluetooth icon is missing or Bluetooth can't be turned on or off, you may want to run the Bluetooth troubleshooter.</span></span> <span data-ttu-id="ac2cf-104">[U okviru Pronalaženje i rešavanje drugih problema](ms-settings:troubleshoot)izaberite **stavku** Rešavanje problema u odeljku Rešavanje problema , a zatim izaberite stavku **Pokreni alatku za rešavanje problema.** </span><span class="sxs-lookup"><span data-stu-id="ac2cf-104">[Open the Troubleshoot settings](ms-settings:troubleshoot), click **Bluetooth** under **Find and fix other problems**, click **Run the troubleshooter**.</span></span>

<span data-ttu-id="ac2cf-105">Ako ne vidite ikonu Bluetooth, ali se Bluetooth pojavljuje u upravljaču uređajima:</span><span class="sxs-lookup"><span data-stu-id="ac2cf-105">If you don't see the Bluetooth icon, but Bluetooth does appear in Device Manager:</span></span>

1. <span data-ttu-id="ac2cf-106">U upravljaču uređajima izaberite **stavku Bluetooth**.</span><span class="sxs-lookup"><span data-stu-id="ac2cf-106">In Device Manager, click **Bluetooth**.</span></span> <span data-ttu-id="ac2cf-107">Pritisnite i držite ime Bluetooth adaptera (ili kliknite desnim tasterom miša na njegovo ime) i **izaberite stavku Deinstalni uređaj.**</span><span class="sxs-lookup"><span data-stu-id="ac2cf-107">Press and hold (or right-click) the Bluetooth adapter name and click **Uninstall device**.</span></span>

2. <span data-ttu-id="ac2cf-108">Zatvorite Windows uređaj, sačekajte nekoliko sekundi, a zatim ga ponovo uključite.</span><span class="sxs-lookup"><span data-stu-id="ac2cf-108">Shut down your Windows device, wait a few seconds, and then turn it back on.</span></span> <span data-ttu-id="ac2cf-109">Windows će pokušati da ponovo instalira upravljački program.</span><span class="sxs-lookup"><span data-stu-id="ac2cf-109">Windows will try to reinstall the driver.</span></span>

<span data-ttu-id="ac2cf-110">Ako ste nedavno instalirali ispravke za Windows 10 ili nadogradili na Windows 10, možda ćete želeti da proverite da li postoje ispravke upravljačkih programa:</span><span class="sxs-lookup"><span data-stu-id="ac2cf-110">If you recently installed Windows 10 updates or upgraded to Windows 10, you may want to check for driver updates:</span></span>

1. <span data-ttu-id="ac2cf-111">U upravljaču uređajima izaberite **stavku Bluetooth**, a zatim kliknite na ime Bluetooth adaptera (što može da sadrži reč "radio").</span><span class="sxs-lookup"><span data-stu-id="ac2cf-111">In Device Manager, click **Bluetooth**, and then click the Bluetooth adapter name (which may include the word "radio").</span></span>

2. <span data-ttu-id="ac2cf-112">Pritisnite i držite Bluetooth adapter (ili kliknite desnim tasterom miša na taj bluetooth adapter), a zatim izaberite stavku Automatski ažuriraj pretragu upravljačkog programa za  >  **ažurirani softver upravljačkog programa.**</span><span class="sxs-lookup"><span data-stu-id="ac2cf-112">Press and hold (or right-click) the Bluetooth adapter, and then click **Update driver** > **Search automatically for updated driver software**.</span></span> <span data-ttu-id="ac2cf-113">Sledite korake, a zatim kliknite **na dugme Zatvori**.</span><span class="sxs-lookup"><span data-stu-id="ac2cf-113">Follow the steps, then click **Close**.</span></span>

      - <span data-ttu-id="ac2cf-114">Ako Windows ne može da pronađe novi Bluetooth upravljački program, posetite veb sajt proizvođača računara i odatle preuzmite najnoviji Bluetooth upravljački program.</span><span class="sxs-lookup"><span data-stu-id="ac2cf-114">If Windows can't find a new Bluetooth driver, visit the PC manufacturer's website and download the latest Bluetooth driver from there.</span></span>

    - <span data-ttu-id="ac2cf-115">Kada ga preuzmete, izaberite stavku Ažuriraj upravljački program Potraži softver upravljačkog programa na računaru Potražite lokaciju na kojoj su datoteke upravljačkog programa uskladištene > U redu Dalje i pratite   >  **korake** za  >     >  instalaciju.</span><span class="sxs-lookup"><span data-stu-id="ac2cf-115">After you download it, click **Update driver** > **Browse my computer for driver software** > **Browse** for the location where the driver files are stored > **OK** > **Next**, and follow the steps to install.</span></span>

3. <span data-ttu-id="ac2cf-116">Kada instalirate ažurirani upravljački program, ponovo pokrenite računar, a zatim proverite da li to rešava problem sa vezom.</span><span class="sxs-lookup"><span data-stu-id="ac2cf-116">After installing the updated driver, restart the machine, and then check whether that fixes the connection issue.</span></span>

<span data-ttu-id="ac2cf-117">Za više detalja o tome kako da rešite probleme sa Bluetooth 10, pogledajte ceo članak Rešavanje problema sa [Bluetooth 10 operativnim sistemom](https://support.microsoft.com/help/14169/windows-10-fix-bluetooth-problems).</span><span class="sxs-lookup"><span data-stu-id="ac2cf-117">For more details of how to troubleshoot Bluetooth problems, please see the full article, [Fix Bluetooth problems in Windows 10](https://support.microsoft.com/help/14169/windows-10-fix-bluetooth-problems).</span></span>
