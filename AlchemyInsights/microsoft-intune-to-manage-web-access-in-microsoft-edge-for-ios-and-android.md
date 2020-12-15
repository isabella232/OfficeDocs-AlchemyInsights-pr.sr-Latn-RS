---
title: Korišćenje Microsoft Intune za upravljanje Veb pristupom u usluzi Microsoft Edge za iOS i android
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
ms.openlocfilehash: 4d6ab4df4ff9588ce5052421602e347c76c91c3f
ms.sourcegitcommit: a7952283882d341515623d5ae58eda14d0553449
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 12/10/2020
ms.locfileid: "49679606"
---
# <a name="use-microsoft-intune-to-manage-web-access-in-microsoft-edge-for-ios-and-android"></a><span data-ttu-id="976c5-102">Korišćenje Microsoft Intune za upravljanje Veb pristupom u usluzi Microsoft Edge za iOS i android</span><span class="sxs-lookup"><span data-stu-id="976c5-102">Use Microsoft Intune to manage web access in Microsoft Edge for iOS and Android</span></span>

<span data-ttu-id="976c5-103">Microsoft Edge za iOS i Android omogućava korisniku da potraži Veb iz više zasebnih profila.</span><span class="sxs-lookup"><span data-stu-id="976c5-103">Microsoft Edge for iOS and Android lets a user browse the web from multiple, completely separate profiles.</span></span>

<span data-ttu-id="976c5-104">Najbolje usluge zaštite za Microsoft 365 podaci postaju dostupne kada se pretplatite na Enterprise mobilnost + bezbednosni paket, što obuhvata Microsoft Intune i Azure Active Directory Premium funkcije, kao što je uslovno pristup.</span><span class="sxs-lookup"><span data-stu-id="976c5-104">The broadest protection capabilities for Microsoft 365 data become available when you subscribe to the Enterprise Mobility + Security suite, which includes Microsoft Intune and Azure Active Directory Premium features, such as conditional access.</span></span> <span data-ttu-id="976c5-105">U najmanju ruku, želite da primenite uslovno pristupačne smernice koje (1) omogućava korisnicima da se povežu sa mobilnim uređajima na Microsoft Edge za iOS i Android i da (2) sprovodi smernice za zaštitu u aplikaciji Microsoft.</span><span class="sxs-lookup"><span data-stu-id="976c5-105">At a minimum, you’ll want to deploy a conditional access policy that (1) lets users connect from mobile devices to Microsoft Edge for iOS and Android and that (2) implements a Microsoft Intune app-protection policy that provides a protected browsing experience.</span></span>

<span data-ttu-id="976c5-106">Da biste razumeli kako možete da koristite uslovno pristup i smernice, pogledajte članak:</span><span class="sxs-lookup"><span data-stu-id="976c5-106">To understand how you can use conditional access and policies, see:</span></span>

[<span data-ttu-id="976c5-107">Primenjivanje Azure Active Directory uslovnog Access smernica</span><span class="sxs-lookup"><span data-stu-id="976c5-107">Apply Azure Active Directory conditional access policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132481)

[<span data-ttu-id="976c5-108">Kreiranje smernica za zaštitu aplikacije Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="976c5-108">Create Microsoft Intune app protection policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132651)

[<span data-ttu-id="976c5-109">Korišćenje jedinstvenog prijavljivanja za Azure Active Directory – povezane Veb aplikacije u pregledačima zaštićenim smernicama</span><span class="sxs-lookup"><span data-stu-id="976c5-109">Use single sign-on for Azure Active Directory–connected web apps in policy-protected browsers</span></span>](https://go.microsoft.com/fwlink/?linkid=2132482)

[<span data-ttu-id="976c5-110">Korišćenje konfiguracije aplikacije za upravljanje iskustvom pregledanja</span><span class="sxs-lookup"><span data-stu-id="976c5-110">Use app configuration to manage the browsing experience</span></span>](https://go.microsoft.com/fwlink/?linkid=2132483)

[<span data-ttu-id="976c5-111">Omogućavanje korišćenja samo poslovnih i školskih naloga</span><span class="sxs-lookup"><span data-stu-id="976c5-111">Allow the use of only work and school accounts</span></span>](https://go.microsoft.com/fwlink/?linkid=2132652)

[<span data-ttu-id="976c5-112">Primena smernica za konfiguraciju opštih aplikacija</span><span class="sxs-lookup"><span data-stu-id="976c5-112">Deploy general app configuration policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132653)

[<span data-ttu-id="976c5-113">Primena smernica za konfiguraciju aplikacije za zaštitu podataka</span><span class="sxs-lookup"><span data-stu-id="976c5-113">Deploy app configuration policies for data protection</span></span>](https://go.microsoft.com/fwlink/?linkid=2132654)

[<span data-ttu-id="976c5-114">Korišćenje Microsoft krajnjeg Pointa za primenu smernica konfiguracije aplikacija</span><span class="sxs-lookup"><span data-stu-id="976c5-114">Use Microsoft Endpoint Manager to deploy app configuration policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132707)

<span data-ttu-id="976c5-115">Da biste saznali kako da pristupite kontrolisanim evidenciji aplikacija, pogledajte članak [Korišćenje Microsoft Edge za iOS i Android za pristup kontrolisanim evidenciji aplikacija](https://go.microsoft.com/fwlink/?linkid=2132578).</span><span class="sxs-lookup"><span data-stu-id="976c5-115">To learn how to access managed app logs, see [Use Microsoft Edge for iOS and Android to access managed app logs](https://go.microsoft.com/fwlink/?linkid=2132578).</span></span>
