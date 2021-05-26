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
ms.openlocfilehash: b9369b2c2ca31f7d2fceac37ef1e2252b82e933b
ms.sourcegitcommit: 0c104e2bd34ccc09bcea389e470692e92bcf1f8f
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 05/26/2021
ms.locfileid: "52657943"
---
# <a name="configure-endpoint-dlp"></a><span data-ttu-id="9e934-102">Konfigurisanje DLP-a krajnje tačke</span><span class="sxs-lookup"><span data-stu-id="9e934-102">Configure Endpoint DLP</span></span>

<span data-ttu-id="9e934-103">Microsoft DLP krajnje tačke vam omogućava da proširite DLP zaštitu i mogućnost nadgledanja na osetljive informacije na Windows 10 uređajima.</span><span class="sxs-lookup"><span data-stu-id="9e934-103">Microsoft Endpoint DLP allows you to extend DLP protection and monitoring capability to sensitive information on Windows 10 devices.</span></span> <span data-ttu-id="9e934-104">Nakon što se uređaji postave u upravljanje uređajima, možete da kreirate smernice za DLP da biste na stavke nametnuli radnje zaštite.</span><span class="sxs-lookup"><span data-stu-id="9e934-104">After devices are onboarded into device management, you can create DLP policies to enforce protective actions on items.</span></span> <span data-ttu-id="9e934-105">Istraživač aktivnosti može da se koristi za nadgledanje aktivnosti za osetljive stavke.</span><span class="sxs-lookup"><span data-stu-id="9e934-105">The Activity Explorer can be used to monitor activity for sensitive items.</span></span> <span data-ttu-id="9e934-106">Za više informacija, pogledajte [Postavljanje uređaja u upravljanje uređajima](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span><span class="sxs-lookup"><span data-stu-id="9e934-106">For more info, see [Onboarding devices into device management](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span></span>  

<span data-ttu-id="9e934-107">Da biste počeli da koristite DLP krajnje tačke:</span><span class="sxs-lookup"><span data-stu-id="9e934-107">To get started with Endpoint DLP:</span></span>

- <span data-ttu-id="9e934-108">Uverite se da imate odgovarajuće licenciranje za SKU/pretplate.</span><span class="sxs-lookup"><span data-stu-id="9e934-108">Ensure you have the appropriate SKU/subscriptions licensing.</span></span> <span data-ttu-id="9e934-109">Za više informacija, pogledajte [Licenciranje za SKU/pretplate](/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span><span class="sxs-lookup"><span data-stu-id="9e934-109">For more info, see [SKU/subscriptions licensing](/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span></span>
- <span data-ttu-id="9e934-110">Proverite dozvole potrebne za omogućavanje upravljanja uređajem, pristup stranici za postavljanje ili nadgledanje uključivanja/isključivanja uređaja.</span><span class="sxs-lookup"><span data-stu-id="9e934-110">Check the permissions required to enable device management, access the onboarding page, or turn on/off device monitoring.</span></span> <span data-ttu-id="9e934-111">Za više informacija, pogledajte [Dozvole](/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span><span class="sxs-lookup"><span data-stu-id="9e934-111">For more info, see [Permissions](/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span></span>
- <span data-ttu-id="9e934-112">Postavite uređaje u upravljanje uređajima prateći proceduru za postavljanje uređaja.</span><span class="sxs-lookup"><span data-stu-id="9e934-112">Onboard devices into Device management by following the onboarding devices procedure.</span></span> <span data-ttu-id="9e934-113">Za više informacija, pogledajte [Postavljanje uređaja](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span><span class="sxs-lookup"><span data-stu-id="9e934-113">For more info, see [Onboarding devices](/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span></span> 
- <span data-ttu-id="9e934-114">Kreirajte smernice za DLP da biste zaštitili osetljive stavke.</span><span class="sxs-lookup"><span data-stu-id="9e934-114">Create DLP policies to protect your sensitive items.</span></span> <span data-ttu-id="9e934-115">Informacije potražite u članku [ Scenariji smernica za DLP krajnje tačke](/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).</span><span class="sxs-lookup"><span data-stu-id="9e934-115">For info, see [Endpoint DLP policy scenarios](/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).</span></span>

<span data-ttu-id="9e934-116">Za više informacija o Microsoft DLP-u krajnje tačke, pogledajte članak [Saznajte više o Microsoft 365 sprečavanju gubitka podataka krajnje tačke (pregled)](/microsoft-365/compliance/endpoint-dlp-learn-about).</span><span class="sxs-lookup"><span data-stu-id="9e934-116">For more information on the Microsoft Endpoint DLP, see [Learn about Microsoft 365 Endpoint data loss prevention (preview)](/microsoft-365/compliance/endpoint-dlp-learn-about).</span></span>

<span data-ttu-id="9e934-117">**Važni koraci za prikupljanje podataka, ako je potrebna podrška:**</span><span class="sxs-lookup"><span data-stu-id="9e934-117">**Important Data Collection steps, if Support is needed:**</span></span>

1. <span data-ttu-id="9e934-118">Preuzmite [pregled MDATP klijenta Analyzer](https://aka.ms/betamdatpanalyzer).</span><span class="sxs-lookup"><span data-stu-id="9e934-118">Download [MDATP Client Analyzer Preview](https://aka.ms/betamdatpanalyzer).</span></span>
1. <span data-ttu-id="9e934-119">Koristite alatku kao administrator iz cmd prozora:</span><span class="sxs-lookup"><span data-stu-id="9e934-119">Run the tool as Admin from the cmd window:</span></span>

    <span data-ttu-id="9e934-120">**MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t**</span><span class="sxs-lookup"><span data-stu-id="9e934-120">**MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t**</span></span>

1. <span data-ttu-id="9e934-121">Kada vam bude zatraženo **Unesite broj minuta** za prikupljanje praćenja: , unesite broj minuta potrebnih za pokretanje scenarija.</span><span class="sxs-lookup"><span data-stu-id="9e934-121">When prompted with **Enter the number of minutes to collect traces:**, enter the number of minutes required to run the scenario.</span></span>
1. <span data-ttu-id="9e934-122">Pokrenite scenario.</span><span class="sxs-lookup"><span data-stu-id="9e934-122">Run the scenario.</span></span>

<span data-ttu-id="9e934-123">Prikupite izlaz Zip datoteke da biste ga dali agentu za podršku.</span><span class="sxs-lookup"><span data-stu-id="9e934-123">Collect the Zip file output to give to the Support agent.</span></span>
