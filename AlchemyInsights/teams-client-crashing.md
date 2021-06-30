---
title: Teams klijent pada
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
ms.openlocfilehash: 7acb2f5f87a9cfbd67cd94efca696665fd80fc4a
ms.sourcegitcommit: 3cdfde87b7311c200431196031af92c640fd0d8d
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 06/29/2021
ms.locfileid: "53187735"
---
# <a name="teams-client-crashing"></a><span data-ttu-id="3cf28-102">Teams klijent pada</span><span class="sxs-lookup"><span data-stu-id="3cf28-102">Teams client crashing</span></span>

<span data-ttu-id="3cf28-103">Ukoliko Teams klijent otkazuje, pokušajte sledeće:</span><span class="sxs-lookup"><span data-stu-id="3cf28-103">If your Teams client is crashing, try the following:</span></span>

- <span data-ttu-id="3cf28-104">Ako koristite Teams aplikaciju za stone računare, [ uverite se da je aplikacija potpuno ažurirana](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span><span class="sxs-lookup"><span data-stu-id="3cf28-104">If you are using the Teams desktop app, [make sure the app is fully updated](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

- <span data-ttu-id="3cf28-105">Uverite se da [su Microsoft 365 ULS i opsezi](/microsoftteams/connectivity-issues) adresa.</span><span class="sxs-lookup"><span data-stu-id="3cf28-105">Make sure all the [Microsoft 365 URLs and address ranges](/microsoftteams/connectivity-issues) are accessible.</span></span>

- <span data-ttu-id="3cf28-106">Prijavite se na nalog zakupca [](/office365/enterprise/view-service-health) i proverite kontrolnu tablu za zdravstveno stanje usluge kako biste potvrdili da ne postoji preklovanje ili degradacija usluge.</span><span class="sxs-lookup"><span data-stu-id="3cf28-106">Log in with your tenant admin account and check your [Service Health Dashboard](/office365/enterprise/view-service-health) to verify that no outage or service degradation exists.</span></span>

- <span data-ttu-id="3cf28-107">Deinstalujte i ponovo instalirajte aplikaciju Teams aplikaciju</span><span class="sxs-lookup"><span data-stu-id="3cf28-107">Uninstall and reinstall the Teams Application</span></span>
    - <span data-ttu-id="3cf28-108">Potražite fasciklu %appdata%\Microsoft\Teams\ na računaru i izbrišite sve datoteke iz tog direktorijuma.</span><span class="sxs-lookup"><span data-stu-id="3cf28-108">Browse to the %appdata%\Microsoft\Teams\ folder on your computer and delete all files in that directory.</span></span>
    - <span data-ttu-id="3cf28-109">Preuzmite i instalirajte [aplikaciju Teams](https://www.microsoft.com/microsoft-teams/download-app)i, ako je moguće, instalirajte Teams kao administrator (kliknite desnim tasterom miša na instalacioni program za Teams i izaberite stavku Pokreni kao **administrator** ako je dostupno).</span><span class="sxs-lookup"><span data-stu-id="3cf28-109">[Download and install the Teams App](https://www.microsoft.com/microsoft-teams/download-app), and if possible, install Teams as an administrator (right-click the Teams installer, and select **Run as administrator** if available).</span></span>

<span data-ttu-id="3cf28-110">Ako Teams klijent i dalje pada, pokušajte ponovo da predstavite problem.</span><span class="sxs-lookup"><span data-stu-id="3cf28-110">If your Teams client is still crashing, try to reproduce the issue.</span></span> <span data-ttu-id="3cf28-111">Ako možete da:</span><span class="sxs-lookup"><span data-stu-id="3cf28-111">If you can:</span></span>

1. <span data-ttu-id="3cf28-112">Koristite zapisivač koraka da biste uhvatili korake.</span><span class="sxs-lookup"><span data-stu-id="3cf28-112">Use the Steps Recorder to capture your steps.</span></span>
    - <span data-ttu-id="3cf28-113">Zatvorite SVE nepotrebne ili poverljive aplikacije.</span><span class="sxs-lookup"><span data-stu-id="3cf28-113">Close ALL unnecessary or confidential applications.</span></span>
    - <span data-ttu-id="3cf28-114">Pokrenite program za snimanje koraka i ponovo predstavite problem dok ste prijavljeni sa korisničkim nalogom na koji to utiče.</span><span class="sxs-lookup"><span data-stu-id="3cf28-114">Launch the Steps Recorder and reproduce the issue while logged in with the affected user account.</span></span>
    - <span data-ttu-id="3cf28-115">[Prikupljajte evidencije timova koje snimaju snimljene korake repropro.](/microsoftteams/log-files)</span><span class="sxs-lookup"><span data-stu-id="3cf28-115">[Collect the teams logs that capture the recorded repro steps](/microsoftteams/log-files).</span></span> <span data-ttu-id="3cf28-116">**Naznaka:** Proverite da li ste zabeležili adresu za prijavljivanje upečenog korisnika.</span><span class="sxs-lookup"><span data-stu-id="3cf28-116">**Note**: Make sure you capture the sign-in address of the impacted user.</span></span>
    - <span data-ttu-id="3cf28-117">Prikupite informacije o neis kvaru i/ili neispravnu kontejner (Windows).</span><span class="sxs-lookup"><span data-stu-id="3cf28-117">Collect the dump and/or Fault bucket info (Windows).</span></span> <span data-ttu-id="3cf28-118">Pokrenite Windows PowerShell na računaru na kojem je došlo do pada i pokrenite sledeće komande (nakon svake komande pritisnite taster Enter):</span><span class="sxs-lookup"><span data-stu-id="3cf28-118">Launch Windows Powershell on the machine where the crash is occurring and run the following commands (after each command, press Enter):</span></span>

    <span data-ttu-id="3cf28-119">`cd $env:temp` `Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt`</span><span class="sxs-lookup"><span data-stu-id="3cf28-119">`cd $env:temp` `Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt`</span></span>
    `notepad .\FaultBuckets.txt`
    
2. <span data-ttu-id="3cf28-120">Kada se tekstualna datoteka generiše i pojavi na ekranu, sačuvajte je i priložite zahtevu za uslugom.</span><span class="sxs-lookup"><span data-stu-id="3cf28-120">After the text file is generated and appears on your screen, save the file and attach it to the service request.</span></span> 
