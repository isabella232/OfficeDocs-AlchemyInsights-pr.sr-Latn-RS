---
title: Konfiguriši DLP.
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/03/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6108"
- "3200001"
ms.openlocfilehash: 039c8f78c5896b66eab5763fb0bbddd3f0b06f2d
ms.sourcegitcommit: 1dada930649a2625eb6d15910b2bfd5e1e00e5b6
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/03/2020
ms.locfileid: "46556037"
---
# <a name="configure-endpoint-dlp"></a><span data-ttu-id="badde-102">Konfiguriši DLP.</span><span class="sxs-lookup"><span data-stu-id="badde-102">Configure Endpoint DLP</span></span>

<span data-ttu-id="badde-103">DLP Microsoft-krajnja tačka vam omogućava da proširite mogućnosti za zaštitu i nadgledanje DLP-a sa osetljivim informacijama na Windows 10 uređajima.</span><span class="sxs-lookup"><span data-stu-id="badde-103">Microsoft Endpoint DLP allows you to extend DLP protection and monitoring capability to sensitive information on Windows 10 devices.</span></span> <span data-ttu-id="badde-104">Kada se uređaji ukrcnu u upravljanje uređajima, možete da kreirate DLP smernice da biste primenili zaštitne radnje na stavkama.</span><span class="sxs-lookup"><span data-stu-id="badde-104">After devices are onboarded into device management, you can create DLP policies to enforce protective actions on items.</span></span> <span data-ttu-id="badde-105">Istraživač aktivnosti može da se koristi za nadgledanje aktivnosti za osetljive stavke.</span><span class="sxs-lookup"><span data-stu-id="badde-105">The Activity Explorer can be used to monitor activity for sensitive items.</span></span> <span data-ttu-id="badde-106">Više informacija potražite u okviru [uređaja za upravljanje uređajima](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span><span class="sxs-lookup"><span data-stu-id="badde-106">For more info, see [Onboarding devices into device management](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).</span></span>  

<span data-ttu-id="badde-107">Da biste započeli sa DLP krajnjeg čvorišta:</span><span class="sxs-lookup"><span data-stu-id="badde-107">To get started with Endpoint DLP:</span></span>

- <span data-ttu-id="badde-108">Uverite se da imate odgovarajuće licenciranje MJ/pretplata.</span><span class="sxs-lookup"><span data-stu-id="badde-108">Ensure you have the appropriate SKU/subscriptions licensing.</span></span> <span data-ttu-id="badde-109">Više informacija potražite u članku [licenciranje MJ/pretplata](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span><span class="sxs-lookup"><span data-stu-id="badde-109">For more info, see [SKU/subscriptions licensing](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).</span></span>
- <span data-ttu-id="badde-110">Proverite dozvole koje su potrebne da biste omogućili upravljanje uređajima, pristupite stranici onintersa ili uključite/isključite nadgledanje uređaja.</span><span class="sxs-lookup"><span data-stu-id="badde-110">Check the permissions required to enable device management, access the onboarding page, or turn on/off device monitoring.</span></span> <span data-ttu-id="badde-111">Više informacija potražite u članku [dozvole](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span><span class="sxs-lookup"><span data-stu-id="badde-111">For more info, see [Permissions](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).</span></span>
- <span data-ttu-id="badde-112">Na one uređaje u "upravljanje uređajima" prateći postupak "onsurfuređaje".</span><span class="sxs-lookup"><span data-stu-id="badde-112">Onboard devices into Device management by following the onboarding devices procedure.</span></span> <span data-ttu-id="badde-113">Ako nedostaje opcija za uređaj za ukrcavanje (pregled) pod M365 **postavkama**usaglašenosti, potvrdite da imate odgovarajuću licencu i dozvole navedene iznad.</span><span class="sxs-lookup"><span data-stu-id="badde-113">If you're missing the Device Onboarding (preview) option under M365 Compliance  **Settings**, confirm you have the appropriate license and permissions referenced above.</span></span> <span data-ttu-id="badde-114">Više informacija potražite u članku [Uređaji za ukrcavanje](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span><span class="sxs-lookup"><span data-stu-id="badde-114">For more info, see [Onboarding devices](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices).</span></span> 
- <span data-ttu-id="badde-115">Kreirajte "DLP" smernice da biste zaštitili osetljive stavke.</span><span class="sxs-lookup"><span data-stu-id="badde-115">Create DLP policies to protect your sensitive items.</span></span> <span data-ttu-id="badde-116">Više informacija potražite u okviru [scenarija smernica za DLP](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).</span><span class="sxs-lookup"><span data-stu-id="badde-116">For info, see [Endpoint DLP policy scenarios](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).</span></span>

<span data-ttu-id="badde-117">Za više informacija o DLL-u na krajnjoj tački Microsoft-a, pogledajte članak [Saznajte o sprečavanju gubitka podataka za microsoft 365 na krajnjoj tački (pregled)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).</span><span class="sxs-lookup"><span data-stu-id="badde-117">For more information on the Microsoft Endpoint DLP, see [Learn about Microsoft 365 Endpoint data loss prevention (preview)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).</span></span>