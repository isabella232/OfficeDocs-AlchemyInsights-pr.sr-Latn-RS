---
title: Teams klijent otkazuje?
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
- "9002323"
- "4512"
ms.openlocfilehash: 20f03b075787cab85ab15d5272c0416b88ebbaee
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826285"
---
# <a name="teams-client-crashing"></a><span data-ttu-id="a9908-102">Teams klijent otkazuje?</span><span class="sxs-lookup"><span data-stu-id="a9908-102">Teams client crashing?</span></span>

<span data-ttu-id="a9908-103">Ukoliko Teams klijent otkazuje, pokušajte sledeće:</span><span class="sxs-lookup"><span data-stu-id="a9908-103">If your Teams client is crashing, try the following:</span></span>

- <span data-ttu-id="a9908-104">Ako koristite Teams aplikaciju za stone računare, [ uverite se da je aplikacija potpuno ažurirana](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span><span class="sxs-lookup"><span data-stu-id="a9908-104">If you are using the Teams desktop app, [make sure the app is fully updated](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

- <span data-ttu-id="a9908-105">Uverite se da su [svi Microsoft 365 UL adrese i opsezi](https://docs.microsoft.com/microsoftteams/connectivity-issues) adresa pristupačni.</span><span class="sxs-lookup"><span data-stu-id="a9908-105">Make sure all the [Microsoft 365 URLs and address ranges](https://docs.microsoft.com/microsoftteams/connectivity-issues) are accessible.</span></span>

- <span data-ttu-id="a9908-106">Prijavite se na nalog zakupca [](https://docs.microsoft.com/office365/enterprise/view-service-health) i proverite kontrolnu tablu za zdravstveno stanje usluge kako biste potvrdili da ne postoji preklovanje ili degradacija usluge.</span><span class="sxs-lookup"><span data-stu-id="a9908-106">Log in with your tenant admin account and check your [Service Health Dashboard](https://docs.microsoft.com/office365/enterprise/view-service-health) to verify that no outage or service degradation exists.</span></span>

- <span data-ttu-id="a9908-107">Deinstalacija i poništite instaliranje Teams aplikacije (veza)</span><span class="sxs-lookup"><span data-stu-id="a9908-107">Uninstall and reinstall the Teams Application (link)</span></span>
    - <span data-ttu-id="a9908-108">Potražite fasciklu %appdata%\Microsoft\teams\ na računaru i izbrišite sve datoteke iz tog direktorijuma.</span><span class="sxs-lookup"><span data-stu-id="a9908-108">Browse to the %appdata%\Microsoft\teams\ folder on your computer and delete all files in that directory.</span></span>
    - <span data-ttu-id="a9908-109">Preuzmite i [instalirajte Aplikaciju Teams](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy)i, ako je moguće, instalirajte Teams kao administrator (kliknite desnim tasterom miša na Teams instalacioni program i izaberite stavku "Pokreni kao administrator" ako je dostupno).</span><span class="sxs-lookup"><span data-stu-id="a9908-109">[Download and install the Teams App](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy), and if possible, install Teams as an administrator (right click the Teams installer and select "Run as administrator" if available).</span></span>

<span data-ttu-id="a9908-110">Ako Teams klijent i dalje pada, možete li ponovo da predstavite problem?</span><span class="sxs-lookup"><span data-stu-id="a9908-110">If your Teams client is still crashing, can you reproduce the issue?</span></span> <span data-ttu-id="a9908-111">Ako je tako:</span><span class="sxs-lookup"><span data-stu-id="a9908-111">If so:</span></span>

1. <span data-ttu-id="a9908-112">Koristite zapisivač koraka da biste uhvatili korake.</span><span class="sxs-lookup"><span data-stu-id="a9908-112">Use the Steps Recorder to capture your steps.</span></span>
    - <span data-ttu-id="a9908-113">Zatvorite SVE nepotrebne ili poverljive aplikacije.</span><span class="sxs-lookup"><span data-stu-id="a9908-113">Close ALL unnecessary or confidential applications.</span></span>
    - <span data-ttu-id="a9908-114">Pokrenite program za snimanje koraka i ponovo predstavite problem dok ste prijavljeni sa korisničkim nalogom na koji to utiče.</span><span class="sxs-lookup"><span data-stu-id="a9908-114">Launch the Steps Recorder and reproduce the issue while logged in with the affected user account.</span></span>
    - <span data-ttu-id="a9908-115">[Prikupljajte evidencije timova koje snimaju snimljene korake repropro.](https://docs.microsoft.com/microsoftteams/log-files)</span><span class="sxs-lookup"><span data-stu-id="a9908-115">[Collect the teams logs that capture the recorded repro steps](https://docs.microsoft.com/microsoftteams/log-files).</span></span> <span data-ttu-id="a9908-116">**Naznaka:** Proverite da li ste zabeležili adresu za prijavljivanje upečenog korisnika.</span><span class="sxs-lookup"><span data-stu-id="a9908-116">**Note**: Make sure you capture the sign-in address of the impacted user.</span></span>
    - <span data-ttu-id="a9908-117">Prikupite informacije o neiskladu i/ili neispravnoj kontejnneru (Windows).</span><span class="sxs-lookup"><span data-stu-id="a9908-117">Collect the dump and/or Fault bucket info (Windows).</span></span> <span data-ttu-id="a9908-118">Pokrenite Windows PowerShell na računaru na kom je došlo do pada i pokrenite sledeće komande:</span><span class="sxs-lookup"><span data-stu-id="a9908-118">Launch Windows Powershell on the machine where the crash is occurring and run the following commands:</span></span>

        `
        PS C:\Users\user01> cd $env:temp
        PS C:\Users\user01\AppData\Local\Temp> Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt
        PS C:\Users\user01\AppData\Local\Temp> notepad .\FaultBuckets.txt
        `
    
2. <span data-ttu-id="a9908-119">Priložite datoteku na slučaj podrške.</span><span class="sxs-lookup"><span data-stu-id="a9908-119">Attach the file to your support case.</span></span>
