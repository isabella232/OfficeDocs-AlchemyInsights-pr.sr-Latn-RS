---
title: Oslobodite prostor za disk jedinicu u operativnom sistemu Windows 10
ms.author: pebaum
author: pebaum
manager: dansimp
ms.date: 03/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9771"
- "9005403"
ms.openlocfilehash: 3838f3db3bc5f54bcb1a2558484056f3194b76e1
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037947"
---
# <a name="free-up-drive-space-in-windows-10"></a><span data-ttu-id="4b258-102">Oslobodite prostor za disk jedinicu u operativnom sistemu Windows 10</span><span class="sxs-lookup"><span data-stu-id="4b258-102">Free up drive space in Windows 10</span></span>

<span data-ttu-id="4b258-103">Evo dve opcije da biste oslobodili prostor za disk jedinicu u operativnom sistemu Windows:</span><span class="sxs-lookup"><span data-stu-id="4b258-103">Here are two options to free up drive space in Windows:</span></span>

- <span data-ttu-id="4b258-104">Oslobodite prostor za disk jedinicu u operativnom sistemu Windows 10.</span><span class="sxs-lookup"><span data-stu-id="4b258-104">Free up drive space in Windows 10.</span></span>
- <span data-ttu-id="4b258-105">Oslobodite prostor za Windows 10 ispravke sa spoljnim uređajem za skladištenje.</span><span class="sxs-lookup"><span data-stu-id="4b258-105">Free up space for Windows 10 updates with external storage device.</span></span>

<span data-ttu-id="4b258-106">Ako i dalje imate nizak prostor na disku nakon korišćenja alatke "Čišćenje diska", moguće je da se fascikla temp brzo popunjava sa datotekama aplikacije (. appx) koje koristi Microsoft Store.</span><span class="sxs-lookup"><span data-stu-id="4b258-106">If you still have low disk space after using Disk Cleanup, it’s possible that your Temp folder is quickly filling up with application (.appx) files used by Microsoft Store.</span></span> <span data-ttu-id="4b258-107">Da biste rešili ovaj problem, poništite skladište, obrišite keš skladišta, a zatim pokrenite alatku za rešavanje problema sa uslugom Windows Update.</span><span class="sxs-lookup"><span data-stu-id="4b258-107">To fix this problem, reset the Store, clear the Store cache, and then run the Windows Update troubleshooter.</span></span> <span data-ttu-id="4b258-108">Uverite se da je Microsoft prodavnica zatvorena pre nego što nastavite sa ovim koracima.</span><span class="sxs-lookup"><span data-stu-id="4b258-108">Make sure Microsoft Store is closed before you proceed with these steps.</span></span>

<span data-ttu-id="4b258-109">**1. prvi: poništavanje Microsoft prodavnice**</span><span class="sxs-lookup"><span data-stu-id="4b258-109">**Step 1: Reset Microsoft Store**</span></span>

<span data-ttu-id="4b258-110">**Napomena** Ovo trajno briše podatke aplikacije na uređaju, uključujući željene postavke i detalje za prijavljivanje.</span><span class="sxs-lookup"><span data-stu-id="4b258-110">**Note** This permanently deletes the app data on the device, including your preferences and sign-in details.</span></span>

1. <span data-ttu-id="4b258-111">Izaberite stavke postavke **početnog**  >  **postavki**  >    >  **& funkcijama**.</span><span class="sxs-lookup"><span data-stu-id="4b258-111">Select **Start** > **Settings** > **Apps** > **Apps & features**.</span></span>

1. <span data-ttu-id="4b258-112">Na listi aplikacija pronađite i izaberite stavku Microsoft butik.</span><span class="sxs-lookup"><span data-stu-id="4b258-112">In the list of apps, locate and select Microsoft Store.</span></span>

1. <span data-ttu-id="4b258-113">Izaberite stavku **Napredne opcije**.</span><span class="sxs-lookup"><span data-stu-id="4b258-113">Select **Advanced options**.</span></span>

1. <span data-ttu-id="4b258-114">Pomerajte se nadole i izaberite stavku **Poništi**, a zatim **potvrdite početne vrednosti**.</span><span class="sxs-lookup"><span data-stu-id="4b258-114">Scroll down and select **Reset**, and then **Confirm Reset**.</span></span>

<span data-ttu-id="4b258-115">**2.2: Opozovite izbor u okviru keš Microsoft prodavnice**</span><span class="sxs-lookup"><span data-stu-id="4b258-115">**Step 2: Clear the Microsoft Store cache**</span></span>

1. <span data-ttu-id="4b258-116">Pritisnite taster sa Windows logotipom + R da biste otvorili dijalog "pokreće".</span><span class="sxs-lookup"><span data-stu-id="4b258-116">Press the Windows Logo Key + R to open the Run dialog box.</span></span>

1. <span data-ttu-id="4b258-117">Otkucajte wsreset.exe i kliknite na **dugme u redu**.</span><span class="sxs-lookup"><span data-stu-id="4b258-117">Type wsreset.exe and select **OK**.</span></span>

1. <span data-ttu-id="4b258-118">Otvara se prazan prozor komandne linije.</span><span class="sxs-lookup"><span data-stu-id="4b258-118">A blank Command Prompt window opens.</span></span> <span data-ttu-id="4b258-119">Posle 10 sekundi, prozor se zatvara i automatski se otvara.</span><span class="sxs-lookup"><span data-stu-id="4b258-119">After about 10 seconds, the window closes and the Store opens automatically.</span></span>

<span data-ttu-id="4b258-120">**Treći broj: poništi Windows Update**</span><span class="sxs-lookup"><span data-stu-id="4b258-120">**Step 3: Reset Windows Update**</span></span>

1. <span data-ttu-id="4b258-121">Izaberite stavku **pokretanje**  >  **postavki**  >  **Ažuriranje & bezbednosti**  >  .</span><span class="sxs-lookup"><span data-stu-id="4b258-121">Select **Start** > **Settings** > **Update & Security** > **Troubleshoot**.</span></span>

1. <span data-ttu-id="4b258-122">Pomerajte se nadole i izaberite stavku **Windows Update** sa liste i izaberite stavku **pokrenite alatku za rešavanje problema**.</span><span class="sxs-lookup"><span data-stu-id="4b258-122">Scroll down and select **Windows Update** from the list, and select **Run the troubleshooter**.</span></span>

1. <span data-ttu-id="4b258-123">Ponovo pokrenite računar i provjerite da li i dalje nailazite na problem.</span><span class="sxs-lookup"><span data-stu-id="4b258-123">Reboot your computer and check whether you're still experiencing the issue.</span></span>

