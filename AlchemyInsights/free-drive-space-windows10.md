---
title: Oslobađanje prostora na disk jedinici na OS Windows 10
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
- "9774"
- "9005390"
- "9005403"
ms.openlocfilehash: 2313636307bfddce2810c2d4c4ce9e3b407a7bdf
ms.sourcegitcommit: 7b2e5078dd65f11af6650e692a7ea48e91f544e0
ms.translationtype: HT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/02/2021
ms.locfileid: "51505370"
---
# <a name="free-up-drive-space-in-windows-10"></a><span data-ttu-id="f58e3-102">Oslobađanje prostora na disk jedinici na OS Windows 10</span><span class="sxs-lookup"><span data-stu-id="f58e3-102">Free up drive space in Windows 10</span></span>

<span data-ttu-id="f58e3-103">Ovo su dve opcije za oslobađanje prostora na disk jedinici na OS Windows:</span><span class="sxs-lookup"><span data-stu-id="f58e3-103">Here are two options to free up drive space in Windows:</span></span>

- <span data-ttu-id="f58e3-104">Oslobodite prostor na disk jedinici na OS Windows 10.</span><span class="sxs-lookup"><span data-stu-id="f58e3-104">Free up drive space in Windows 10.</span></span>
- <span data-ttu-id="f58e3-105">Oslobodite prostor za Windows 10 ispravke sa spoljnim uređajem za skladištenje.</span><span class="sxs-lookup"><span data-stu-id="f58e3-105">Free up space for Windows 10 updates with external storage device.</span></span>

<span data-ttu-id="f58e3-106">Ako i dalje nemate dovoljno prostora na disku nakon čišćenja diska, moguće je da se fascikla privremenih datoteka brzo puni datotekama aplikacija (.appx) koje koristi Microsoft Store prodavnica.</span><span class="sxs-lookup"><span data-stu-id="f58e3-106">If you still have low disk space after using Disk Cleanup, it’s possible that your Temp folder is quickly filling up with application (.appx) files used by Microsoft Store.</span></span> <span data-ttu-id="f58e3-107">Da biste rešili ovaj problem, resetujte Store prodavnicu, obrišite keš memoriju Store prodavnice, a zatim pokrenite rešavanje problema veb lokacije Windows Update.</span><span class="sxs-lookup"><span data-stu-id="f58e3-107">To fix this problem, reset the Store, clear the Store cache, and then run the Windows Update troubleshooter.</span></span> <span data-ttu-id="f58e3-108">Proverite da li je Microsoft Store prodavnica zatvorena pre nego što nastavite sa ovim koracima.</span><span class="sxs-lookup"><span data-stu-id="f58e3-108">Make sure Microsoft Store is closed before you proceed with these steps.</span></span>

<span data-ttu-id="f58e3-109">**1. korak: Resetujte Microsoft Store**</span><span class="sxs-lookup"><span data-stu-id="f58e3-109">**Step 1: Reset Microsoft Store**</span></span>

<span data-ttu-id="f58e3-110">**Napomena** Ovo trajno briše podatke aplikacija na uređaju, uključujući i željene postavke i detalje o prijavljivanju.</span><span class="sxs-lookup"><span data-stu-id="f58e3-110">**Note** This permanently deletes the app data on the device, including your preferences and sign-in details.</span></span>

1. <span data-ttu-id="f58e3-111">Izaberite **ekran „Početak“** > **Postavke** > **Aplikacije** > **Aplikacije i funkcije**.</span><span class="sxs-lookup"><span data-stu-id="f58e3-111">Select **Start** > **Settings** > **Apps** > **Apps & features**.</span></span>

1. <span data-ttu-id="f58e3-112">Na listi aplikacija pronađite i izaberite Microsoft Store prodavnicu.</span><span class="sxs-lookup"><span data-stu-id="f58e3-112">In the list of apps, locate and select Microsoft Store.</span></span>

1. <span data-ttu-id="f58e3-113">Izaberite **Napredne opcije**.</span><span class="sxs-lookup"><span data-stu-id="f58e3-113">Select **Advanced options**.</span></span>

1. <span data-ttu-id="f58e3-114">Pomerajte se nadole i izaberite stavku **Resetovanje**, a zatim stavku **Potvrdi resetovanje**.</span><span class="sxs-lookup"><span data-stu-id="f58e3-114">Scroll down and select **Reset**, and then **Confirm Reset**.</span></span>

<span data-ttu-id="f58e3-115">**2. korak: Obrišite keš memoriju Microsoft Store prodavnice**</span><span class="sxs-lookup"><span data-stu-id="f58e3-115">**Step 2: Clear the Microsoft Store cache**</span></span>

1. <span data-ttu-id="f58e3-116">Pritisnite kombinaciju tastera sa Windows logotipom + R da biste otvorili dijalog „Pokretanje“.</span><span class="sxs-lookup"><span data-stu-id="f58e3-116">Press the Windows Logo Key + R to open the Run dialog box.</span></span>

1. <span data-ttu-id="f58e3-117">Otkucajte wsreset.exe i izaberite stavku **U redu**.</span><span class="sxs-lookup"><span data-stu-id="f58e3-117">Type wsreset.exe and select **OK**.</span></span>

1. <span data-ttu-id="f58e3-118">Otvara se prazan prozor komandne linije.</span><span class="sxs-lookup"><span data-stu-id="f58e3-118">A blank Command Prompt window opens.</span></span> <span data-ttu-id="f58e3-119">Nakon oko 10 sekundi, prozor se zatvara a Store prodavnica se automatski otvara.</span><span class="sxs-lookup"><span data-stu-id="f58e3-119">After about 10 seconds, the window closes and the Store opens automatically.</span></span>

<span data-ttu-id="f58e3-120">**3. korak: Resetovanje veb lokacije Windows Update**</span><span class="sxs-lookup"><span data-stu-id="f58e3-120">**Step 3: Reset Windows Update**</span></span>

1. <span data-ttu-id="f58e3-121">Izaberite **ekran „Početak“** > **Postavke** > **Ažuriranje i bezbednost** > **Rešavanje problema**.</span><span class="sxs-lookup"><span data-stu-id="f58e3-121">Select **Start** > **Settings** > **Update & Security** > **Troubleshoot**.</span></span>

1. <span data-ttu-id="f58e3-122">Krećite se nadole i izaberite stavku **Veb lokacija Windows Update** sa liste, a zatim izaberite stavku **Pokreni rešavanje problema**.</span><span class="sxs-lookup"><span data-stu-id="f58e3-122">Scroll down and select **Windows Update** from the list, and select **Run the troubleshooter**.</span></span>

1. <span data-ttu-id="f58e3-123">Ponovo pokrenite računar i proverite da li se problem i dalje javlja.</span><span class="sxs-lookup"><span data-stu-id="f58e3-123">Reboot your computer and check whether you're still experiencing the issue.</span></span>

