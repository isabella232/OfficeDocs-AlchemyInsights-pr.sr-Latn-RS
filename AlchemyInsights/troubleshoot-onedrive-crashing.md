---
title: Rešavanje problema sa OneDrive padovima
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003084"
- "5885"
ms.openlocfilehash: 1155d370911b28bbb1ba83a15eace66d1daea28f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47665012"
---
# <a name="troubleshoot-onedrive-crashes"></a><span data-ttu-id="07bc4-102">Rešavanje problema sa OneDrive padovima</span><span class="sxs-lookup"><span data-stu-id="07bc4-102">Troubleshoot OneDrive crashes</span></span>

<span data-ttu-id="07bc4-103">Ako OneDrive više puta pada, isprobajte ove korake za rešavanje problema:</span><span class="sxs-lookup"><span data-stu-id="07bc4-103">If OneDrive repeatedly crashes, try these troubleshooting steps:</span></span>

<span data-ttu-id="07bc4-104">**Obezbedite da nisu podešeni ključevi registratora:**</span><span class="sxs-lookup"><span data-stu-id="07bc4-104">**Ensure registry keys aren’t set:**</span></span>

1. <span data-ttu-id="07bc4-105">Korišćenje uređivača registratora potražite u HKEY_LOCAL_MACHINE \SOFTWARE\Policies\Microsoft\OneDrive</span><span class="sxs-lookup"><span data-stu-id="07bc4-105">Using Registry Editor, navigate to HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive</span></span>
2. <span data-ttu-id="07bc4-106">Ako je funkcija Oneblefilesyncngsc postavljena na 1, otvorite ključ i promenite vrednost u 0.</span><span class="sxs-lookup"><span data-stu-id="07bc4-106">If DisableFileSyncNGSC is present and set to 1, open the key and change the value to 0.</span></span>
3. <span data-ttu-id="07bc4-107">Ručno pokretanje usluge OneDrive tako što ćete početi</span><span class="sxs-lookup"><span data-stu-id="07bc4-107">Manually launch OneDrive by going to Start</span></span> ![Pritisnite taster Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="07bc4-109">, u polju za pretragu otkucajte OneDrive, a zatim kliknite na OneDrive aplikaciju za računare.</span><span class="sxs-lookup"><span data-stu-id="07bc4-109">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="07bc4-110">**Poništavanje OneDrive:**</span><span class="sxs-lookup"><span data-stu-id="07bc4-110">**Reset OneDrive:**</span></span>

<span data-ttu-id="07bc4-111">Primeć</span><span class="sxs-lookup"><span data-stu-id="07bc4-111">Notes:</span></span>

- <span data-ttu-id="07bc4-112">Ponovno podešavanje usluge OneDrive prekida sve postojeće veze sinhronizacije (uključujući lični OneDrive ako je podešeno).</span><span class="sxs-lookup"><span data-stu-id="07bc4-112">Resetting OneDrive disconnects all your existing sync connections (including your personal OneDrive if set up).</span></span>
- <span data-ttu-id="07bc4-113">Nećete izgubiti datoteke ili podatke tako što ćete ponovo postaviti OneDrive na računaru.</span><span class="sxs-lookup"><span data-stu-id="07bc4-113">You won't lose files or data by resetting OneDrive on your computer.</span></span>

<span data-ttu-id="07bc4-114">**Da biste poništili OneDrive:**</span><span class="sxs-lookup"><span data-stu-id="07bc4-114">**To reset OneDrive:**</span></span>

1. <span data-ttu-id="07bc4-115">Otvorite dijalog "pokreće" tako što ćete pritisnuti taster Windows Key i R.</span><span class="sxs-lookup"><span data-stu-id="07bc4-115">Open a Run dialog by pressing Windows key    and R.</span></span>
2. <span data-ttu-id="07bc4-116">Otkucajte% LocalAppData% \Microsoft\OneDrive\onedrive.exe/reset i pritisnite u redu.</span><span class="sxs-lookup"><span data-stu-id="07bc4-116">Type %localappdata%\Microsoft\OneDrive\onedrive.exe /reset and press OK.</span></span> <span data-ttu-id="07bc4-117">Prozor sa komandama može da se pojavi nakratko.</span><span class="sxs-lookup"><span data-stu-id="07bc4-117">A Command window may appear briefly.</span></span>
3. <span data-ttu-id="07bc4-118">Ručno pokretanje usluge OneDrive tako što ćete početi</span><span class="sxs-lookup"><span data-stu-id="07bc4-118">Manually launch OneDrive by going to Start</span></span> ![Pritisnite taster Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="07bc4-120">, u polju za pretragu otkucajte OneDrive, a zatim kliknite na OneDrive aplikaciju za računare.</span><span class="sxs-lookup"><span data-stu-id="07bc4-120">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="07bc4-121">Primeć</span><span class="sxs-lookup"><span data-stu-id="07bc4-121">Notes:</span></span>

- <span data-ttu-id="07bc4-122">Ako ste odabrali da sinhronizujete samo neke fascikle pre ponovnog početnih vrednosti, moraćete to ponovo da uradite kada se sinhronizacija dovrši.</span><span class="sxs-lookup"><span data-stu-id="07bc4-122">If you had chosen to sync only some folders before the reset, you will need to do that again once sync has completed.</span></span> <span data-ttu-id="07bc4-123">Pročitajte [stavku Odaberite koje OneDrive fascikle želite da sinhronizujete sa računarom](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)   za više informacija.</span><span class="sxs-lookup"><span data-stu-id="07bc4-123">Read [Choose which OneDrive folders to sync to your computer](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85) for more information.</span></span>
- <span data-ttu-id="07bc4-124">Moraćete da dovršite ovo za ličnu OneDrive i OneDrive for Business.</span><span class="sxs-lookup"><span data-stu-id="07bc4-124">You will need to complete this for your personal OneDrive and OneDrive for Business.</span></span>