---
title: Rešavanje problema sa OneDrive padovima
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003084"
- "5885"
ms.openlocfilehash: 7fbc4617a0426eb11359339edc950a108f782750
ms.sourcegitcommit: 462522e6bccde76f6c46795b0eca71320c5d442d
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 06/15/2020
ms.locfileid: "44749167"
---
# <a name="troubleshoot-onedrive-crashes"></a><span data-ttu-id="3d6a0-102">Rešavanje problema sa OneDrive padovima</span><span class="sxs-lookup"><span data-stu-id="3d6a0-102">Troubleshoot OneDrive crashes</span></span>

<span data-ttu-id="3d6a0-103">Ako OneDrive više puta padne, isprobajte ove korake za rešavanje problema:</span><span class="sxs-lookup"><span data-stu-id="3d6a0-103">If OneDrive repeatedly crashes, try these troubleshooting steps:</span></span>

<span data-ttu-id="3d6a0-104">**Uverite se da ključevi registratora nisu podešeni:**</span><span class="sxs-lookup"><span data-stu-id="3d6a0-104">**Ensure registry keys aren’t set:**</span></span>

1. <span data-ttu-id="3d6a0-105">Pomoću programa Registry Editor Krećite se do HKEY_LOCAL_MACHINE \SOFTWARE\Policies\Microsoft\OneDrive</span><span class="sxs-lookup"><span data-stu-id="3d6a0-105">Using Registry Editor, navigate to HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive</span></span>
2. <span data-ttu-id="3d6a0-106">Ako je DisableFileSyncNGSC prisutan i postavljen na 1, otvorite ključ i promenite vrednost u 0.</span><span class="sxs-lookup"><span data-stu-id="3d6a0-106">If DisableFileSyncNGSC is present and set to 1, open the key and change the value to 0.</span></span>
3. <span data-ttu-id="3d6a0-107">Ručno pokretanje usluge OneDrive tako što ćete otići na početni ekran</span><span class="sxs-lookup"><span data-stu-id="3d6a0-107">Manually launch OneDrive by going to Start</span></span> ![Pritisnite taster sa Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="3d6a0-109">Otkucajte OneDrive u polju za pretragu, a zatim kliknite na aplikaciju OneDrive radne površine.</span><span class="sxs-lookup"><span data-stu-id="3d6a0-109">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="3d6a0-110">**Poništi OneDrive:**</span><span class="sxs-lookup"><span data-stu-id="3d6a0-110">**Reset OneDrive:**</span></span>

<span data-ttu-id="3d6a0-111">Beleške:</span><span class="sxs-lookup"><span data-stu-id="3d6a0-111">Notes:</span></span>

- <span data-ttu-id="3d6a0-112">Uspostavljanje početnih vrednosti usluge OneDrive prekida vezu sa svim postojećim sinhronizovanim vezama (uključujući i vašu ličnu OneDrive ako je podešeno).</span><span class="sxs-lookup"><span data-stu-id="3d6a0-112">Resetting OneDrive disconnects all your existing sync connections (including your personal OneDrive if set up).</span></span>
- <span data-ttu-id="3d6a0-113">Datoteke ili podatke nećete izgubiti tako što ćete ponovo da pokrenete OneDrive na računaru.</span><span class="sxs-lookup"><span data-stu-id="3d6a0-113">You won't lose files or data by resetting OneDrive on your computer.</span></span>

<span data-ttu-id="3d6a0-114">**Da biste uspostavili početne vrednosti usluge OneDrive:**</span><span class="sxs-lookup"><span data-stu-id="3d6a0-114">**To reset OneDrive:**</span></span>

1. <span data-ttu-id="3d6a0-115">Otvorite dijalog "pokretanje" tako što ćete pritisnuti Windows taster i R.</span><span class="sxs-lookup"><span data-stu-id="3d6a0-115">Open a Run dialog by pressing Windows key    and R.</span></span>
2. <span data-ttu-id="3d6a0-116">Otkucajte% LocalAppData% \Microsoft\OneDrive\onedrive.exe/reset i Pritisnite OK.</span><span class="sxs-lookup"><span data-stu-id="3d6a0-116">Type %localappdata%\Microsoft\OneDrive\onedrive.exe /reset and press OK.</span></span> <span data-ttu-id="3d6a0-117">Moguće je da će komandni prozor biti nakratko prikazan.</span><span class="sxs-lookup"><span data-stu-id="3d6a0-117">A Command window may appear briefly.</span></span>
3. <span data-ttu-id="3d6a0-118">Ručno pokretanje usluge OneDrive tako što ćete otići na početni ekran</span><span class="sxs-lookup"><span data-stu-id="3d6a0-118">Manually launch OneDrive by going to Start</span></span> ![Pritisnite taster sa Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="3d6a0-120">Otkucajte OneDrive u polju za pretragu, a zatim kliknite na aplikaciju OneDrive radne površine.</span><span class="sxs-lookup"><span data-stu-id="3d6a0-120">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="3d6a0-121">Beleške:</span><span class="sxs-lookup"><span data-stu-id="3d6a0-121">Notes:</span></span>

- <span data-ttu-id="3d6a0-122">Ako ste odabrali da sinhronizujete samo neke fascikle pre nego što uspostavite početne vrednosti, biće potrebno da to uradite ponovo kada se sinhronizacija dovrši.</span><span class="sxs-lookup"><span data-stu-id="3d6a0-122">If you had chosen to sync only some folders before the reset, you will need to do that again once sync has completed.</span></span> <span data-ttu-id="3d6a0-123">Pročitajte [izbor koje OneDrive fascikle želite da sinhronizujete sa računarom](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)da biste   dobili više informacija.</span><span class="sxs-lookup"><span data-stu-id="3d6a0-123">Read [Choose which OneDrive folders to sync to your computer](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85) for more information.</span></span>
- <span data-ttu-id="3d6a0-124">Ovo ćete morati da dovršite za vaše lične usluge OneDrive i OneDrive za posao.</span><span class="sxs-lookup"><span data-stu-id="3d6a0-124">You will need to complete this for your personal OneDrive and OneDrive for Business.</span></span>