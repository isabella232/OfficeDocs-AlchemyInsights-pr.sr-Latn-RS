---
title: Rešavanje Bluetooth problema u operativnom sistemu Windows 10
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
- "9001475"
- "3506"
ms.openlocfilehash: 7e7a397a1f6777972a81bcbb6bffa1c98d8370a4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47730173"
---
# <a name="fix-bluetooth-problems-in-windows-10"></a><span data-ttu-id="0ccb3-102">Rešavanje Bluetooth problema u operativnom sistemu Windows 10</span><span class="sxs-lookup"><span data-stu-id="0ccb3-102">Fix Bluetooth problems in Windows 10</span></span>

<span data-ttu-id="0ccb3-103">Ako nedostaje Bluetooth ikona ili Bluetooth nije moguće uključiti ili isključiti, možda ćete želeti da pokrenete Bluetooth program za rešavanje problema.</span><span class="sxs-lookup"><span data-stu-id="0ccb3-103">If the Bluetooth icon is missing or Bluetooth can't be turned on or off, you may want to run the Bluetooth troubleshooter.</span></span> <span data-ttu-id="0ccb3-104">[Otvorite postavke rešavanja problema](ms-settings:troubleshoot), kliknite na **Bluetooth** u okviru **Pronalaženje i rešavanje drugih problema**, izaberite stavku **pokrenite alatku za rešavanje problema**.</span><span class="sxs-lookup"><span data-stu-id="0ccb3-104">[Open the Troubleshoot settings](ms-settings:troubleshoot), click **Bluetooth** under **Find and fix other problems**, click **Run the troubleshooter**.</span></span>

<span data-ttu-id="0ccb3-105">Ako ne vidite ikonu Bluetooth, ali se Bluetooth pojavljuje u alatki "Upravljač uređajima":</span><span class="sxs-lookup"><span data-stu-id="0ccb3-105">If you don't see the Bluetooth icon, but Bluetooth does appear in Device Manager:</span></span>

1. <span data-ttu-id="0ccb3-106">U alatki Upravljač uređajima kliknite na **Bluetooth**.</span><span class="sxs-lookup"><span data-stu-id="0ccb3-106">In Device Manager, click **Bluetooth**.</span></span> <span data-ttu-id="0ccb3-107">Pritisnite i držite (ili kliknite desnim tasterom miša na) ime Bluetooth adaptera i izaberite stavku **Deinstaliraj uređaj**.</span><span class="sxs-lookup"><span data-stu-id="0ccb3-107">Press and hold (or right-click) the Bluetooth adapter name and click **Uninstall device**.</span></span>

2. <span data-ttu-id="0ccb3-108">Isključite Windows uređaj, sačekajte nekoliko sekundi, a zatim ga ponovo uključite.</span><span class="sxs-lookup"><span data-stu-id="0ccb3-108">Shut down your Windows device, wait a few seconds, and then turn it back on.</span></span> <span data-ttu-id="0ccb3-109">Windows će pokušati da ponovo instalira upravljački program.</span><span class="sxs-lookup"><span data-stu-id="0ccb3-109">Windows will try to reinstall the driver.</span></span>

<span data-ttu-id="0ccb3-110">Ako ste nedavno instalirali Windows 10 ispravke ili nadogradili na Windows 10, možda ćete želeti da potražite ispravke upravljačkih programa:</span><span class="sxs-lookup"><span data-stu-id="0ccb3-110">If you recently installed Windows 10 updates or upgraded to Windows 10, you may want to check for driver updates:</span></span>

1. <span data-ttu-id="0ccb3-111">U upravljaču uređajima kliknite na **Bluetooth**, a zatim izaberite ime Bluetooth adaptera (koje može da ukljuci reč "radio").</span><span class="sxs-lookup"><span data-stu-id="0ccb3-111">In Device Manager, click **Bluetooth**, and then click the Bluetooth adapter name (which may include the word "radio").</span></span>

2. <span data-ttu-id="0ccb3-112">Pritisnite i držite Bluetooth adapter (ili kliknite desnim tasterom miša na nju), a zatim izaberite stavku **Ažuriraj upravljački program**  >  **automatski za ažurirani softver upravljačkog programa**.</span><span class="sxs-lookup"><span data-stu-id="0ccb3-112">Press and hold (or right-click) the Bluetooth adapter, and then click **Update driver** > **Search automatically for updated driver software**.</span></span> <span data-ttu-id="0ccb3-113">Slijedite korake, a zatim kliknite na dugme **Zatvori**.</span><span class="sxs-lookup"><span data-stu-id="0ccb3-113">Follow the steps, then click **Close**.</span></span>

      - <span data-ttu-id="0ccb3-114">Ako Windows ne može da pronađe novi Bluetooth upravljački program, posetite Veb lokaciju proizvođača računara i preuzmite najnoviji Bluetooth upravljački program odande.</span><span class="sxs-lookup"><span data-stu-id="0ccb3-114">If Windows can't find a new Bluetooth driver, visit the PC manufacturer's website and download the latest Bluetooth driver from there.</span></span>

    - <span data-ttu-id="0ccb3-115">Kada je preuzmete, izaberite stavku **Ažuriraj upravljački program**  >  **Potraži softver za upravljački program**  >  **potražite** na lokaciji na kojoj se skladište upravljački programi > **u redu**  >  **sledeće**i slijedite korake za instaliranje.</span><span class="sxs-lookup"><span data-stu-id="0ccb3-115">After you download it, click **Update driver** > **Browse my computer for driver software** > **Browse** for the location where the driver files are stored > **OK** > **Next**, and follow the steps to install.</span></span>

3. <span data-ttu-id="0ccb3-116">Kada instalirate ažurirani upravljački program, ponovo pokrenite računar, a zatim potvrdite da li to rešava problem povezivanja.</span><span class="sxs-lookup"><span data-stu-id="0ccb3-116">After installing the updated driver, restart the machine, and then check whether that fixes the connection issue.</span></span>

<span data-ttu-id="0ccb3-117">Da biste saznali više o tome kako da rešite probleme sa Bluetooth, pogledajte ceo članak, [rešite Bluetooth probleme u operativnom sistemu Windows 10](https://support.microsoft.com/help/14169/windows-10-fix-bluetooth-problems).</span><span class="sxs-lookup"><span data-stu-id="0ccb3-117">For more details of how to troubleshoot Bluetooth problems, please see the full article, [Fix Bluetooth problems in Windows 10](https://support.microsoft.com/help/14169/windows-10-fix-bluetooth-problems).</span></span>
