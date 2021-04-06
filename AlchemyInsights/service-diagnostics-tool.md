---
title: Alatka za dijagnostiku usluge za Windows virtuelnu radnu površinu
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9004219"
- "10873"
ms.openlocfilehash: dfa59c86508c8658c880f4f3f21a002524e909d1
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/05/2021
ms.locfileid: "51595861"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a><span data-ttu-id="1d799-102">Alatka za dijagnostiku usluge za Windows virtuelnu radnu površinu</span><span class="sxs-lookup"><span data-stu-id="1d799-102">Service diagnostics tool for Windows Virtual Desktop</span></span>

<span data-ttu-id="1d799-103">Windows virtuelna radna površina (WVD) nudi dijagnostičnu alatku koja omogućava adminiistantima da identifikuju greške putem jednog interfejsa.</span><span class="sxs-lookup"><span data-stu-id="1d799-103">Windows Virtual Desktop (WVD) offers a diagnostic tool that lets admins identify errors through a single interface.</span></span> <span data-ttu-id="1d799-104">Ova alatka evidentljuje informacije vezane za dijagnostiku svaki put kada neko dodelite WVD ulogu.</span><span class="sxs-lookup"><span data-stu-id="1d799-104">This tool logs diagnostics-related info whenever WVD is used by someone assigned a WVD role.</span></span> <span data-ttu-id="1d799-105">Svaka evidencija sadrži informacije o Ulozi VDD uključenoj u aktivnosti, porukama o grešci koje se pojavljuju tokom sesije i informacijama o zakupca i korisniku.</span><span class="sxs-lookup"><span data-stu-id="1d799-105">Each log contains info about the WVD role involved in the activity, the error messages that appear during the session, and the info about the tenant and user.</span></span> <span data-ttu-id="1d799-106">Azure analitika evidencije može da se konfiguriše tako što će pratiti ove korake za hvatanje evidencije aktivnosti koju kreira dijagnostička alatka:</span><span class="sxs-lookup"><span data-stu-id="1d799-106">Azure Log Analytics can be configured to capture the activity log created by the diagnostic tool by following these steps:</span></span>

1. <span data-ttu-id="1d799-107">Kreirajte radni prostor anatike evidencije uz [Azure portal](https://go.microsoft.com/fwlink/?linkid=2129500) ili [Azure PowerShell.](https://go.microsoft.com/fwlink/?linkid=2129501)</span><span class="sxs-lookup"><span data-stu-id="1d799-107">Create a Log Analytics workspace with the [Azure portal](https://go.microsoft.com/fwlink/?linkid=2129500) or [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).</span></span>

1. <span data-ttu-id="1d799-108">[Povežite Windows računare sa Azure monitorom.](https://go.microsoft.com/fwlink/?linkid=2129913)</span><span class="sxs-lookup"><span data-stu-id="1d799-108">[Connect Windows computers to Azure Monitor](https://go.microsoft.com/fwlink/?linkid=2129913).</span></span> <span data-ttu-id="1d799-109">Nabavite ID radnog prostora i primarni ključ radnog prostora.</span><span class="sxs-lookup"><span data-stu-id="1d799-109">Get the Workspace ID and the Primary Key of your workspace.</span></span> <span data-ttu-id="1d799-110">Čarobnjaku za podešavanje su potrebne ove informacije da bi ispravno konfigurisao agenta i da bi mogao da komunicira sa uslugom Azure Monitor.</span><span class="sxs-lookup"><span data-stu-id="1d799-110">The setup wizard needs this info to properly configure the agent and to ensure it can communicate with Azure Monitor.</span></span>

1. <span data-ttu-id="1d799-111">[Push diagnostics data to your workspace](https://go.microsoft.com/fwlink/?linkid=2128284).</span><span class="sxs-lookup"><span data-stu-id="1d799-111">[Push diagnostics data to your workspace](https://go.microsoft.com/fwlink/?linkid=2128284).</span></span> <span data-ttu-id="1d799-112">Podatke o dijagnostici možete da gurate od WVD zakupca do ankete evidencije za radni prostor.</span><span class="sxs-lookup"><span data-stu-id="1d799-112">You can push diagnostics data from your WVD tenant to the Log Analytics for your workspace.</span></span>

1. <span data-ttu-id="1d799-113">[Identifikujte i dijagnostiku](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell) problema koji su unutrašnji ili spoljni u odnosu na WVD.</span><span class="sxs-lookup"><span data-stu-id="1d799-113">[Identify and diagnose](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell) issues that are internal or external in relation to WVD.</span></span>

<span data-ttu-id="1d799-114">Da biste saznali više o konfigurisanju alatke za dijagnostiku usluge za WVD, pogledajte korišćenje anatike evidencije za funkciju dijagnostike.</span><span class="sxs-lookup"><span data-stu-id="1d799-114">To learn more about configuring the service diagnostics tool for WVD, see Use Log Analytics for the diagnostics feature.</span></span>