---
title: Rešavanje problema sa padima u usluzi OneDrive
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003084"
- "5885"
ms.openlocfilehash: 4bf45e7780dcbabb95b3eecfb2df55beffde11d6
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826213"
---
# <a name="troubleshoot-onedrive-crashes"></a><span data-ttu-id="b8a6f-102">Rešavanje problema sa padima u usluzi OneDrive</span><span class="sxs-lookup"><span data-stu-id="b8a6f-102">Troubleshoot OneDrive crashes</span></span>

<span data-ttu-id="b8a6f-103">Ako OneDrive više puta pada, isprobajte ove korake za rešavanje problema:</span><span class="sxs-lookup"><span data-stu-id="b8a6f-103">If OneDrive repeatedly crashes, try these troubleshooting steps:</span></span>

<span data-ttu-id="b8a6f-104">**Uverite se da ključevi registratora nisu podešeni:**</span><span class="sxs-lookup"><span data-stu-id="b8a6f-104">**Ensure registry keys aren’t set:**</span></span>

1. <span data-ttu-id="b8a6f-105">Pomoću uređivača registratora pređite na HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive</span><span class="sxs-lookup"><span data-stu-id="b8a6f-105">Using Registry Editor, navigate to HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive</span></span>
2. <span data-ttu-id="b8a6f-106">Ako je postavka DisableFileSyncNGSC prisutna i postavljena na 1, otvorite ključ i promenite vrednost na 0.</span><span class="sxs-lookup"><span data-stu-id="b8a6f-106">If DisableFileSyncNGSC is present and set to 1, open the key and change the value to 0.</span></span>
3. <span data-ttu-id="b8a6f-107">Ručno pokrenite OneDrive tako što ćete otvoriti "Start" meni</span><span class="sxs-lookup"><span data-stu-id="b8a6f-107">Manually launch OneDrive by going to Start</span></span> ![Pritisnite taster Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="b8a6f-109">, otkucajte OneDrive u polju za pretragu, a zatim kliknite na OneDrive aplikaciju za računare.</span><span class="sxs-lookup"><span data-stu-id="b8a6f-109">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="b8a6f-110">**Uspostavite početne vrednosti za OneDrive:**</span><span class="sxs-lookup"><span data-stu-id="b8a6f-110">**Reset OneDrive:**</span></span>

<span data-ttu-id="b8a6f-111">Napomene:</span><span class="sxs-lookup"><span data-stu-id="b8a6f-111">Notes:</span></span>

- <span data-ttu-id="b8a6f-112">Uspostavljanje početnih vrednosti za OneDrive prekida sve postojeće veze sinhronizacije (uključujući lični OneDrive ako je podešen).</span><span class="sxs-lookup"><span data-stu-id="b8a6f-112">Resetting OneDrive disconnects all your existing sync connections (including your personal OneDrive if set up).</span></span>
- <span data-ttu-id="b8a6f-113">Nećete izgubiti datoteke ili podatke resetujući OneDrive na računaru.</span><span class="sxs-lookup"><span data-stu-id="b8a6f-113">You won't lose files or data by resetting OneDrive on your computer.</span></span>

<span data-ttu-id="b8a6f-114">**Da biste uspostavili početne vrednosti za OneDrive:**</span><span class="sxs-lookup"><span data-stu-id="b8a6f-114">**To reset OneDrive:**</span></span>

1. <span data-ttu-id="b8a6f-115">Otvorite dijalog "Pokretanje" tako što biste pritisnuli Taster Windows i R.</span><span class="sxs-lookup"><span data-stu-id="b8a6f-115">Open a Run dialog by pressing Windows key    and R.</span></span>
2. <span data-ttu-id="b8a6f-116">Ukucaj %localappdata%\Microsoft\OneDrive\onedrive.exe /reset i kliknite na dugme U redu.</span><span class="sxs-lookup"><span data-stu-id="b8a6f-116">Type %localappdata%\Microsoft\OneDrive\onedrive.exe /reset and press OK.</span></span> <span data-ttu-id="b8a6f-117">Komandni prozor može se pojaviti nakratko.</span><span class="sxs-lookup"><span data-stu-id="b8a6f-117">A Command window may appear briefly.</span></span>
3. <span data-ttu-id="b8a6f-118">Ručno pokrenite OneDrive tako što ćete otvoriti "Start" meni</span><span class="sxs-lookup"><span data-stu-id="b8a6f-118">Manually launch OneDrive by going to Start</span></span> ![Pritisnite taster Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="b8a6f-120">, otkucajte OneDrive u polju za pretragu, a zatim kliknite na OneDrive aplikaciju za računare.</span><span class="sxs-lookup"><span data-stu-id="b8a6f-120">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="b8a6f-121">Napomene:</span><span class="sxs-lookup"><span data-stu-id="b8a6f-121">Notes:</span></span>

- <span data-ttu-id="b8a6f-122">Ako ste odabrali da sinhronizujete samo neke fascikle pre reset pošte, morate to da uradite ponovo kada se sinhronizacija završi.</span><span class="sxs-lookup"><span data-stu-id="b8a6f-122">If you had chosen to sync only some folders before the reset, you will need to do that again once sync has completed.</span></span> <span data-ttu-id="b8a6f-123">Pročitajte [stavku Odaberite koje Fascikle za OneDrive treba sinhronizovati sa računarom](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)   za više informacija.</span><span class="sxs-lookup"><span data-stu-id="b8a6f-123">Read [Choose which OneDrive folders to sync to your computer](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85) for more information.</span></span>
- <span data-ttu-id="b8a6f-124">Morate ovo da dovršite za lični OneDrive i OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="b8a6f-124">You will need to complete this for your personal OneDrive and OneDrive for Business.</span></span>