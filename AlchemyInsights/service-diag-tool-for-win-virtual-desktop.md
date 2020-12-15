---
title: Alatka za dijagnostiku usluge za Windows virtuelnu radnu površinu
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003893"
- "6947"
ms.openlocfilehash: c2e6f7fbcddc6721425840e87202a165cdb22664
ms.sourcegitcommit: 87bf574162e536003164ff9af50005c5a7dce601
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 12/14/2020
ms.locfileid: "49680230"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a><span data-ttu-id="47c25-102">Alatka za dijagnostiku usluge za Windows virtuelnu radnu površinu</span><span class="sxs-lookup"><span data-stu-id="47c25-102">Service diagnostics tool for Windows Virtual Desktop</span></span>

<span data-ttu-id="47c25-103">Windows virtuelna radna površina (WVD) nudi dijagnostičku alatku koja omogućava administratori da identifikuju greške kroz jedan interfejs.</span><span class="sxs-lookup"><span data-stu-id="47c25-103">Windows Virtual Desktop (WVD) offers a diagnostic tool that lets admins identify errors through a single interface.</span></span> <span data-ttu-id="47c25-104">Ova alatka evidentira informacije vezane za dijagnostiku kad god WVD koristi neko ko mu je dodeljen.</span><span class="sxs-lookup"><span data-stu-id="47c25-104">This tool logs diagnostics-related info whenever WVD is used by someone assigned a WVD role.</span></span> <span data-ttu-id="47c25-105">Svaka evidencija sadrži informacije o WVD ulozi koja je uključena u aktivnost, poruke o greškama koje se pojavljuju tokom sesije i informacije o zakupcu i korisniku.</span><span class="sxs-lookup"><span data-stu-id="47c25-105">Each log contains info about the WVD role involved in the activity, the error messages that appear during the session, and the info about the tenant and user.</span></span> <span data-ttu-id="47c25-106">Azure evidencija Analitika može da se konfiguriše za hvatanje evidencije aktivnosti kreirane pomoću alatke za dijagnostiku.</span><span class="sxs-lookup"><span data-stu-id="47c25-106">Azure Log Analytics can be configured to capture the activity log created by the diagnostic tool.</span></span> <span data-ttu-id="47c25-107">Evo kako:</span><span class="sxs-lookup"><span data-stu-id="47c25-107">Here's how:</span></span>

1. <span data-ttu-id="47c25-108">Kreirajte radni prostor evidencije evidentiranja pomoću [Azure portala](https://go.microsoft.com/fwlink/?linkid=2129500) ili [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).</span><span class="sxs-lookup"><span data-stu-id="47c25-108">Create a Log Analytics workspace with the [Azure portal](https://go.microsoft.com/fwlink/?linkid=2129500) or [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).</span></span>
1. <span data-ttu-id="47c25-109">[Povežite Windows računare sa uslugom Azure](https://go.microsoft.com/fwlink/?linkid=2129913).</span><span class="sxs-lookup"><span data-stu-id="47c25-109">[Connect Windows computers to Azure Monitor](https://go.microsoft.com/fwlink/?linkid=2129913).</span></span> <span data-ttu-id="47c25-110">Nabavite ID radnog prostora i primarni ključ radnog prostora.</span><span class="sxs-lookup"><span data-stu-id="47c25-110">Get the Workspace ID and the Primary Key of your workspace.</span></span> <span data-ttu-id="47c25-111">Čarobnjaku za podešavanje potrebne su ove informacije da bi se propisno konfigurisao agent i da osigura komunikaciju sa Azure monitorom.</span><span class="sxs-lookup"><span data-stu-id="47c25-111">The setup wizard needs this info to properly configure the agent and to ensure it can communicate with Azure Monitor.</span></span>
1. <span data-ttu-id="47c25-112">[Pritisnite podatke za dijagnostiku u radni prostor](https://go.microsoft.com/fwlink/?linkid=2128284).</span><span class="sxs-lookup"><span data-stu-id="47c25-112">[Push diagnostics data to your workspace](https://go.microsoft.com/fwlink/?linkid=2128284).</span></span> <span data-ttu-id="47c25-113">Možete da pritisnete podatke iz WVD stanara u analitiku evidencije za radni prostor.</span><span class="sxs-lookup"><span data-stu-id="47c25-113">You can push diagnostics data from your WVD tenant to the Log Analytics for your workspace.</span></span>
1. <span data-ttu-id="47c25-114">[Identifikovanje i Dijagnostikovanje problema](https://go.microsoft.com/fwlink/?linkid=2128338) koji su unutrašnji ili spoljni u odnosu na wvd.</span><span class="sxs-lookup"><span data-stu-id="47c25-114">[Identify and diagnose issues](https://go.microsoft.com/fwlink/?linkid=2128338) that are internal or external in relation to WVD.</span></span>

<span data-ttu-id="47c25-115">Da biste saznali više o konfigurisanju alatke za dijagnostiku usluge za WVD, pogledajte članak [Korišćenje analitike evidencije za funkciju dijagnostike](https://go.microsoft.com/fwlink/?linkid=2128084).</span><span class="sxs-lookup"><span data-stu-id="47c25-115">To learn more about configuring the service diagnostics tool for WVD, see [Use Log Analytics for the diagnostics feature](https://go.microsoft.com/fwlink/?linkid=2128084).</span></span>
