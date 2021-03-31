---
title: Konfigurisanje DLP-a krajnje tačke
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6108"
- "3200001"
ms.openlocfilehash: 36af769b67f8c9aa4b8d17e9f4f3f3b82c8a8534
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: HT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/29/2021
ms.locfileid: "51402451"
---
# <a name="configure-endpoint-dlp"></a><span data-ttu-id="a07bd-102">Konfigurisanje DLP-a krajnje tačke</span><span class="sxs-lookup"><span data-stu-id="a07bd-102">Configure Endpoint DLP</span></span>

<span data-ttu-id="a07bd-103">Microsoft DLP krajnje tačke vam omogućava da proširite DLP zaštitu i mogućnost nadgledanja na osetljive informacije na Windows 10 uređajima.</span><span class="sxs-lookup"><span data-stu-id="a07bd-103">Microsoft Endpoint DLP allows you to extend DLP protection and monitoring capability to sensitive information on Windows 10 devices.</span></span> <span data-ttu-id="a07bd-104">Nakon što se uređaji postave u upravljanje uređajima, možete da kreirate smernice za DLP da biste na stavke nametnuli radnje zaštite.</span><span class="sxs-lookup"><span data-stu-id="a07bd-104">After devices are onboarded into device management, you can create DLP policies to enforce protective actions on items.</span></span> <span data-ttu-id="a07bd-105">Istraživač aktivnosti može da se koristi za nadgledanje aktivnosti za osetljive stavke.</span><span class="sxs-lookup"><span data-stu-id="a07bd-105">The Activity Explorer can be used to monitor activity for sensitive items.</span></span> <span data-ttu-id="a07bd-106">Za više informacija, pogledajte [Postavljanje uređaja u upravljanje uređajima](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span><span class="sxs-lookup"><span data-stu-id="a07bd-106">For more info, see [Onboarding devices into device management](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span></span>  

<span data-ttu-id="a07bd-107">Da biste počeli da koristite DLP krajnje tačke:</span><span class="sxs-lookup"><span data-stu-id="a07bd-107">To get started with Endpoint DLP:</span></span>

- <span data-ttu-id="a07bd-108">Uverite se da imate odgovarajuće licenciranje za SKU/pretplate.</span><span class="sxs-lookup"><span data-stu-id="a07bd-108">Ensure you have the appropriate SKU/subscriptions licensing.</span></span> <span data-ttu-id="a07bd-109">Za više informacija, pogledajte [Licenciranje za SKU/pretplate](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span><span class="sxs-lookup"><span data-stu-id="a07bd-109">For more info, see [SKU/subscriptions licensing](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span></span>
- <span data-ttu-id="a07bd-110">Proverite dozvole potrebne za omogućavanje upravljanja uređajem, pristup stranici za postavljanje ili nadgledanje uključivanja/isključivanja uređaja.</span><span class="sxs-lookup"><span data-stu-id="a07bd-110">Check the permissions required to enable device management, access the onboarding page, or turn on/off device monitoring.</span></span> <span data-ttu-id="a07bd-111">Za više informacija, pogledajte [Dozvole](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span><span class="sxs-lookup"><span data-stu-id="a07bd-111">For more info, see [Permissions](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span></span>
- <span data-ttu-id="a07bd-112">Postavite uređaje u upravljanje uređajima prateći proceduru za postavljanje uređaja.</span><span class="sxs-lookup"><span data-stu-id="a07bd-112">Onboard devices into Device management by following the onboarding devices procedure.</span></span> <span data-ttu-id="a07bd-113">Ako vam nedostaje opcija (pregleda) postavljanja uređaja u okviru **Smernica** za M365 usaglašenost, potvrdite da imate odgovarajuću licencu i dozvole na koje se upućuje iznad.</span><span class="sxs-lookup"><span data-stu-id="a07bd-113">If you're missing the Device Onboarding (preview) option under M365 Compliance  **Settings**, confirm you have the appropriate license and permissions referenced above.</span></span> <span data-ttu-id="a07bd-114">Za više informacija, pogledajte [Postavljanje uređaja](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span><span class="sxs-lookup"><span data-stu-id="a07bd-114">For more info, see [Onboarding devices](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span></span> 
- <span data-ttu-id="a07bd-115">Kreirajte smernice za DLP da biste zaštitili osetljive stavke.</span><span class="sxs-lookup"><span data-stu-id="a07bd-115">Create DLP policies to protect your sensitive items.</span></span> <span data-ttu-id="a07bd-116">Informacije potražite u članku [ Scenariji smernica za DLP krajnje tačke](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios &preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="a07bd-116">For info, see [Endpoint DLP policy scenarios](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios &preserve-view=true).</span></span>

<span data-ttu-id="a07bd-117">Za više informacija o Microsoft DLP-u krajnje tačke, pogledajte članak [Saznajte više o Microsoft 365 sprečavanju gubitka podataka krajnje tačke (pregled)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).</span><span class="sxs-lookup"><span data-stu-id="a07bd-117">For more information on the Microsoft Endpoint DLP, see [Learn about Microsoft 365 Endpoint data loss prevention (preview)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).</span></span>

<span data-ttu-id="a07bd-118">**Važni koraci za prikupljanje podataka, ako je potrebna podrška:**</span><span class="sxs-lookup"><span data-stu-id="a07bd-118">**Important Data Collection steps, if Support is needed:**</span></span>

1. <span data-ttu-id="a07bd-119">Preuzmite pregled analizatora MDATP klijenta sa [https://aka.ms/betamdatpanalyzer](https://aka.ms/betamdatpanalyzer "https://aka.ms/betamdatpanalyzer")</span><span class="sxs-lookup"><span data-stu-id="a07bd-119">Download MDATP Client Analyzer Preview from [https://aka.ms/betamdatpanalyzer](https://aka.ms/betamdatpanalyzer "https://aka.ms/betamdatpanalyzer")</span></span>
2. <span data-ttu-id="a07bd-120">Koristite alatku kao administrator iz cmd prozora:</span><span class="sxs-lookup"><span data-stu-id="a07bd-120">Run the tool as Admin from the cmd window:</span></span>
3. <span data-ttu-id="a07bd-121">MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t</span><span class="sxs-lookup"><span data-stu-id="a07bd-121">MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t</span></span>
4. <span data-ttu-id="a07bd-122">Kada vam bude zatraženo „Unesite broj minuta da biste prikupili praćenja: “, unesite broj minuta koji je potreban za pokretanje scenarija</span><span class="sxs-lookup"><span data-stu-id="a07bd-122">When prompted with “Enter the number of minutes to collect traces: ", enter the number of minutes that are required to run the scenario</span></span>
5. <span data-ttu-id="a07bd-123">Pokretanje scenarija</span><span class="sxs-lookup"><span data-stu-id="a07bd-123">Run the scenario</span></span>

<span data-ttu-id="a07bd-124">Prikupite izlaz Zip datoteke koji treba predati agentu za podršku.</span><span class="sxs-lookup"><span data-stu-id="a07bd-124">Collect the Zip file output to be given to the Support agent.</span></span>
