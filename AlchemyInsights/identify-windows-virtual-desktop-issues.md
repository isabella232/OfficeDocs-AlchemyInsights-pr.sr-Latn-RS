---
title: Identifikovanje problema sa Windows virtuelnom radnom površinom
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O364
ms.custom:
- "9004219"
- "10871"
ms.openlocfilehash: 1e55d9d579c389dfe731f887a2a08c6234de2787
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/05/2021
ms.locfileid: "51595858"
---
# <a name="identify-windows-virtual-desktop-issues"></a><span data-ttu-id="216a3-102">Identifikovanje problema sa Windows virtuelnom radnom površinom</span><span class="sxs-lookup"><span data-stu-id="216a3-102">Identify Windows Virtual Desktop issues</span></span>

<span data-ttu-id="216a3-103">Windows virtuelna dijagnostika radne površine koristi samo jednu PowerShell cmdlet komandu, ali sadrži mnogo opcionalnih parametara kako bi suzila i izolovao probleme.</span><span class="sxs-lookup"><span data-stu-id="216a3-103">Windows Virtual Desktop Diagnostics uses just one PowerShell cmdlet but contains many optional parameters to help narrow down and isolate issues.</span></span> <span data-ttu-id="216a3-104">Da biste počeli:</span><span class="sxs-lookup"><span data-stu-id="216a3-104">To get started:</span></span> 

1. <span data-ttu-id="216a3-105">Preuzmite i uvezite modul Windows Virtual Desktop PowerShell.</span><span class="sxs-lookup"><span data-stu-id="216a3-105">Download and import the Windows Virtual Desktop PowerShell module.</span></span> <span data-ttu-id="216a3-106">Više detalja možete da [vidite u temi Windows virtuelne radne površine za Windows PowerShell.](https://docs.microsoft.com/powershell/windows-virtual-desktop/overview)</span><span class="sxs-lookup"><span data-stu-id="216a3-106">For details, see [Windows Virtual Desktop Cmdlets for Windows PowerShell](https://docs.microsoft.com/powershell/windows-virtual-desktop/overview).</span></span>

1. <span data-ttu-id="216a3-107">Pokrenite sledeću cmdlet cmdlet da biste se prijavili na svoj nalog:</span><span class="sxs-lookup"><span data-stu-id="216a3-107">Run the following cmdlet to sign in to your account:</span></span>
    
    <span data-ttu-id="216a3-108">Primer: `Add-RdsAccount -DeploymentUrl 'https://rdbroker.wvd.microsoft.com'`</span><span class="sxs-lookup"><span data-stu-id="216a3-108">Example: `Add-RdsAccount -DeploymentUrl 'https://rdbroker.wvd.microsoft.com'`</span></span>

<span data-ttu-id="216a3-109">**NAPOMOGUĆENO:** Svi upiti koji koriste PowerShell moraju da sadrže parametre -UserName ili -ActivityID.</span><span class="sxs-lookup"><span data-stu-id="216a3-109">**NOTE:** All queries using PowerShell must include either the -UserName or -ActivityID parameters.</span></span> <span data-ttu-id="216a3-110">Mogućnosti nadgledanja možete da koristite za [funkciju dijagnostike](https://go.microsoft.com/fwlink/?linkid=2126847)pomoću funkcije evidencije.</span><span class="sxs-lookup"><span data-stu-id="216a3-110">For monitoring capabilities, see Use [Log Analytics for the diagnostics feature](https://go.microsoft.com/fwlink/?linkid=2126847).</span></span>

<span data-ttu-id="216a3-111">Da biste filtrirali aktivnosti dijagnostike po korisniku, pokrenite sledeću cmdlet alatku:</span><span class="sxs-lookup"><span data-stu-id="216a3-111">To filter diagnostic activities by user, run the following cmdlet:</span></span>

<span data-ttu-id="216a3-112">Primer: `Get-RdsDiagnosticActivities -TenantName < tenantName > -UserName < UserUPN >`</span><span class="sxs-lookup"><span data-stu-id="216a3-112">Example: `Get-RdsDiagnosticActivities -TenantName < tenantName > -UserName < UserUPN >`</span></span>

<span data-ttu-id="216a3-113">Postoji lista filtera koje možete da pokrenete da biste dijagnostikovali probleme.</span><span class="sxs-lookup"><span data-stu-id="216a3-113">There is a list of filters you can run to diagnose issues.</span></span> <span data-ttu-id="216a3-114">Da biste saznali više o dijagnostikovanju problema, pogledajte tj. [identifikovanje i dijagnostikovanje problema sa Windows virtuelnom radnom površinom.](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell)</span><span class="sxs-lookup"><span data-stu-id="216a3-114">To learn more about diagnosing issues, see [Identify and diagnose Windows Virtual Desktop issues](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell).</span></span>

<span data-ttu-id="216a3-115">Da biste saznali više o uobičajenim greškama, pogledajte [uobičajene greške senarios](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#common-error-scenarios).</span><span class="sxs-lookup"><span data-stu-id="216a3-115">To learn more about common errors, see [Common errors senarios](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#common-error-scenarios).</span></span>
