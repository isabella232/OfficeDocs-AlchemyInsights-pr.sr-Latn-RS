---
title: Korišćenje usluge Microsoft Intune za upravljanje veb pristupom u pregledaču Microsoft Edge za iOS i Android
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003846"
- "6895"
- "9006502"
- "11144"
ms.openlocfilehash: a6c6f9563933b7cf6b71c4758c29ffd94617c4be
ms.sourcegitcommit: 7a406a3d4680662e81f0056454f7e25fb2f52504
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 06/17/2021
ms.locfileid: "52989688"
---
# <a name="use-microsoft-intune-to-manage-web-access-in-microsoft-edge-for-ios-and-android"></a><span data-ttu-id="261b5-102">Korišćenje usluge Microsoft Intune za upravljanje veb pristupom u pregledaču Microsoft Edge za iOS i Android</span><span class="sxs-lookup"><span data-stu-id="261b5-102">Use Microsoft Intune to manage web access in Microsoft Edge for iOS and Android</span></span>

<span data-ttu-id="261b5-103">Microsoft Edge za iOS i Android korisnicima mogu da pregledaju veb iz više potpuno odvojenih profila.</span><span class="sxs-lookup"><span data-stu-id="261b5-103">Microsoft Edge for iOS and Android lets a user browse the web from multiple, completely separate profiles.</span></span>

<span data-ttu-id="261b5-104">Najšire mogućnosti zaštite za Microsoft 365 podatke postaju dostupne kada se pretplatite na Enterprise Mobility + Security paket, koji obuhvata Microsoft Intune i Azure Active Directory Premium funkcije, kao što su uslovni pristup.</span><span class="sxs-lookup"><span data-stu-id="261b5-104">The broadest protection capabilities for Microsoft 365 data become available when you subscribe to the Enterprise Mobility + Security suite, which includes Microsoft Intune and Azure Active Directory Premium features, such as conditional access.</span></span> <span data-ttu-id="261b5-105">Primena smernica za uslovni pristup koja (1) omogućava korisnicima da se povežu sa mobilnih uređaja na Microsoft Edge za iOS i Android i da (2) primenjuje Microsoft Intune smernice za zaštitu aplikacija koje pružaju zaštićeno iskustvo pregledanja.</span><span class="sxs-lookup"><span data-stu-id="261b5-105">At a minimum, you’ll want to deploy a conditional access policy that (1) lets users connect from mobile devices to Microsoft Edge for iOS and Android and that (2) implements a Microsoft Intune app-protection policy that provides a protected browsing experience.</span></span>

<span data-ttu-id="261b5-106">Da biste razumeli kako možete da koristite uslovni pristup i smernice, pogledajte:</span><span class="sxs-lookup"><span data-stu-id="261b5-106">To understand how you can use conditional access and policies, see:</span></span>

[<span data-ttu-id="261b5-107">Primena smernica za uslovni pristup za Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="261b5-107">Apply Azure Active Directory conditional access policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132481)

[<span data-ttu-id="261b5-108">Kreiranje smernica za zaštitu aplikacije Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="261b5-108">Create Microsoft Intune app protection policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132651)

[<span data-ttu-id="261b5-109">Koristite jedinstveno prijavljivanje za veb aplikacije povezane sa uslugom Azure Active Directory u pregledačima zaštićenim smernicama</span><span class="sxs-lookup"><span data-stu-id="261b5-109">Use single sign-on for Azure Active Directory–connected web apps in policy-protected browsers</span></span>](https://go.microsoft.com/fwlink/?linkid=2132482)

[<span data-ttu-id="261b5-110">Korišćenje konfiguracije aplikacije za upravljanje iskustvom pregledanja</span><span class="sxs-lookup"><span data-stu-id="261b5-110">Use app configuration to manage the browsing experience</span></span>](https://go.microsoft.com/fwlink/?linkid=2132483)

[<span data-ttu-id="261b5-111">Dozvoli korišćenje samo poslovnih i školskih naloga</span><span class="sxs-lookup"><span data-stu-id="261b5-111">Allow the use of only work and school accounts</span></span>](https://go.microsoft.com/fwlink/?linkid=2132652)

[<span data-ttu-id="261b5-112">Primena opštih smernica za konfiguraciju aplikacije</span><span class="sxs-lookup"><span data-stu-id="261b5-112">Deploy general app configuration policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132653)

[<span data-ttu-id="261b5-113">Primena smernica za konfiguraciju aplikacije za zaštitu podataka</span><span class="sxs-lookup"><span data-stu-id="261b5-113">Deploy app configuration policies for data protection</span></span>](https://go.microsoft.com/fwlink/?linkid=2132654)

[<span data-ttu-id="261b5-114">Korišćenje programa Microsoft Endpoint Manager za primenu smernica za konfiguraciju aplikacije</span><span class="sxs-lookup"><span data-stu-id="261b5-114">Use Microsoft Endpoint Manager to deploy app configuration policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132707)

<span data-ttu-id="261b5-115">Da biste saznali kako da pristupite evidencijama kontrolisanih aplikacija, pogledajte članak Korišćenje programa Microsoft Edge za [iOS i Android](https://go.microsoft.com/fwlink/?linkid=2132578)za pristup evidencijama kontrolisanih aplikacija .</span><span class="sxs-lookup"><span data-stu-id="261b5-115">To learn how to access managed app logs, see [Use Microsoft Edge for iOS and Android to access managed app logs](https://go.microsoft.com/fwlink/?linkid=2132578).</span></span>
