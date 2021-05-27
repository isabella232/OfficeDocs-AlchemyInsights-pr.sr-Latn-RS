---
title: Indikatori ne rade pomoću pregledača Edge
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11230"
- "9005470"
ms.openlocfilehash: df62d965e0dc2ddb656571af99b1e4c3cb52ea35
ms.sourcegitcommit: 4b504650e11adb9894c37b6d8608b53f9d5fc13d
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 05/25/2021
ms.locfileid: "52676465"
---
# <a name="indicators-dont-work-using-edge-browser"></a><span data-ttu-id="f9e30-102">Indikatori ne rade pomoću pregledača Edge</span><span class="sxs-lookup"><span data-stu-id="f9e30-102">Indicators don't work using Edge browser</span></span>

<span data-ttu-id="f9e30-103">Kada kreirate indikator, Edge (Smartscreen) ga ne poštuje.</span><span class="sxs-lookup"><span data-stu-id="f9e30-103">After you created an Indicator, it's not honored by Edge (Smartscreen).</span></span> <span data-ttu-id="f9e30-104">Dodatne informacije potražite u [temi Pravljenje indikatora za IP-ove i UL-ove/domene.](/microsoft-365/security/defender-endpoint/indicator-ip-domain)</span><span class="sxs-lookup"><span data-stu-id="f9e30-104">For more information, see [Create indicators for IPs and URLs/domains](/microsoft-365/security/defender-endpoint/indicator-ip-domain).</span></span>

## <a name="step-1-ensure-the-following"></a><span data-ttu-id="f9e30-105">1. korak: Obezbedite sledeće</span><span class="sxs-lookup"><span data-stu-id="f9e30-105">Step 1: Ensure the following</span></span>

- <span data-ttu-id="f9e30-106">Proverite da li je indikator ispravan (nema greške u greškama u IP/URL adresi, odgovarajuća radnja, odgovarajuće RBAC grupe).</span><span class="sxs-lookup"><span data-stu-id="f9e30-106">Verify that the indicator is correct (no typos in IP/URL, correct action, the correct RBAC groups).</span></span>
- <span data-ttu-id="f9e30-107">Sačekajte najmanje 2 časa nakon kreiranja indikatora da biste uzeti u obzir eventualna kašnjenja.</span><span class="sxs-lookup"><span data-stu-id="f9e30-107">Wait the minimum 2 hours after creating the indicator to take into account any possible latency.</span></span>
- <span data-ttu-id="f9e30-108">Potvrdite da su sistemi spremni za microsoft zaštitnik za krajnje tačke.</span><span class="sxs-lookup"><span data-stu-id="f9e30-108">Confirm that the system(s) are onboarded to Microsoft Defender for Endpoint.</span></span>
- <span data-ttu-id="f9e30-109">Potvrdite da sistemi mogu da komuniciraju sa oblakom.</span><span class="sxs-lookup"><span data-stu-id="f9e30-109">Verify that system(s) can communicate with the Cloud.</span></span>
- <span data-ttu-id="f9e30-110">Uverite se da je Smartscreen omogućen i da može da mu se pristupi tako što ćete ići na [sajt za testiranje.](https://demo.smartscreen.msft.net)</span><span class="sxs-lookup"><span data-stu-id="f9e30-110">Verify that Smartscreen is enabled and reachable by going to the [test site](https://demo.smartscreen.msft.net).</span></span>

## <a name="step-2-troubleshoot-the-potential-issue"></a><span data-ttu-id="f9e30-111">2. korak: Rešavanje potencijalnog problema</span><span class="sxs-lookup"><span data-stu-id="f9e30-111">Step 2: Troubleshoot the potential issue</span></span>

- <span data-ttu-id="f9e30-112">Proverite da li klijent ispunjava zahteve.</span><span class="sxs-lookup"><span data-stu-id="f9e30-112">Make sure the client meets the requirements.</span></span> <span data-ttu-id="f9e30-113">Za detalje pogledajte Kreiranje [indikatora za IP-ove i UL-ove/domene.](/microsoft-365/security/defender-endpoint/indicator-ip-domain)</span><span class="sxs-lookup"><span data-stu-id="f9e30-113">For details, see [Create indicators for IPs and URLs/domains](/microsoft-365/security/defender-endpoint/indicator-ip-domain).</span></span>
- <span data-ttu-id="f9e30-114">Proverite da li imate najnoviju verziju pregledača Edge.</span><span class="sxs-lookup"><span data-stu-id="f9e30-114">Make sure you're running the latest version of the Edge browser.</span></span> <span data-ttu-id="f9e30-115">Da biste videli najnoviju verziju, pogledajte [saznajte koju verziju sistema Microsoft Edge imate.](https://support.microsoft.com/microsoft-edge/find-out-which-version-of-microsoft-edge-you-have-c726bee8-c42e-e472-e954-4cf5123497eb)</span><span class="sxs-lookup"><span data-stu-id="f9e30-115">To find out the latest version, see [Find out which version of Microsoft Edge you have](https://support.microsoft.com/microsoft-edge/find-out-which-version-of-microsoft-edge-you-have-c726bee8-c42e-e472-e954-4cf5123497eb).</span></span>
- <span data-ttu-id="f9e30-116">Ponovo pokrenite pregledač Edge.</span><span class="sxs-lookup"><span data-stu-id="f9e30-116">Restart the Edge browser.</span></span>
- <span data-ttu-id="f9e30-117">Odete na sajt za koji ste instalirali indikator.</span><span class="sxs-lookup"><span data-stu-id="f9e30-117">Navigate to the site for which you have setup an indicator.</span></span> <span data-ttu-id="f9e30-118">Ako se lokacija ne pojavi na očekivani način, pređite na 3. korak.</span><span class="sxs-lookup"><span data-stu-id="f9e30-118">If the site does not appear as expected, continue to Step 3.</span></span> 

## <a name="step-3-collect-data"></a><span data-ttu-id="f9e30-119">3. korak: Prikupljanje podataka</span><span class="sxs-lookup"><span data-stu-id="f9e30-119">Step 3: Collect data</span></span>

- <span data-ttu-id="f9e30-120">Prikupljanje **dijagnostičkih podataka za MDEClientAnalyzer.**</span><span class="sxs-lookup"><span data-stu-id="f9e30-120">Collect **MDEClientAnalyzer** diagnostic data.</span></span> <span data-ttu-id="f9e30-121">Uputstva možete da [vidite u članku Problemi sa mašinama za uletanje u Microsoft zaštitnik za krajnju tačku.](issues-with-onboarding-machines.md)</span><span class="sxs-lookup"><span data-stu-id="f9e30-121">For instructions, see [Issues with onboarding machines to Microsoft Defender for Endpoint](issues-with-onboarding-machines.md).</span></span>
- <span data-ttu-id="f9e30-122">Ako vam je udobno da instalirate i prikupljate Fiddler praćenje, pogledajte [telerik Fiddler](http://www.telerik.com/fiddler).</span><span class="sxs-lookup"><span data-stu-id="f9e30-122">If you are comfortable installing and collecting a Fiddler trace, see [Telerik Fiddler](http://www.telerik.com/fiddler).</span></span>
- <span data-ttu-id="f9e30-123">Ako želite uputstva od Microsoft podrške, kliknite na ikonu Podrška ispod da biste otvorili predmet podrške.</span><span class="sxs-lookup"><span data-stu-id="f9e30-123">If you prefer guidance from Microsoft Support, select the Support icon below to open a support case.</span></span>
