---
title: Upravljač krajnjim tačkama – osnovne linije bezbednosti
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10084"
- "6700005"
ms.openlocfilehash: d2a063fdc4929cbee5fef71bfb47ace8f2ba458f
ms.sourcegitcommit: 430d247cb5dd5dc5d1f82d977456558dfd514277
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/29/2021
ms.locfileid: "51421089"
---
# <a name="endpoint-manager---security-baselines"></a><span data-ttu-id="f85eb-102">Upravljač krajnjim tačkama – osnovne linije bezbednosti</span><span class="sxs-lookup"><span data-stu-id="f85eb-102">EndPoint Manager - Security baselines</span></span>

<span data-ttu-id="f85eb-103">Osnove bezbednosti su unapred konfigurisane grupe postavki operativnog sistema Windows koje vam pomažu da primenite bezbednosne postavke koje preporučuju relevantni timovi za bezbednost.</span><span class="sxs-lookup"><span data-stu-id="f85eb-103">Security baselines are pre-configured groups of Windows settings that help you apply the security settings recommended by the relevant security teams.</span></span> <span data-ttu-id="f85eb-104">Ove osnovne linije mogu da se prilagode tako da isporuče samo postavke i vrednosti koje želite.</span><span class="sxs-lookup"><span data-stu-id="f85eb-104">These baselines can be customized to deliver only the settings and values desired.</span></span> <span data-ttu-id="f85eb-105">Više informacija o osnovnim linijama bezbednosti potražite u temi Korišćenje osnovnih podataka o bezbednosti za [konfigurisanje Windows 10 uređaja u aplikaciji Intune.](https://docs.microsoft.com/mem/intune/protect/security-baselines)</span><span class="sxs-lookup"><span data-stu-id="f85eb-105">For more information about security baselines, see [Use security baselines to configure Windows 10 devices in Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines).</span></span>

<span data-ttu-id="f85eb-106">Trenutno postoje osnovne linije za ove proizvode:</span><span class="sxs-lookup"><span data-stu-id="f85eb-106">There are currently baselines for these products:</span></span>

- <span data-ttu-id="f85eb-107">Windows MDM bezbednosne postavke</span><span class="sxs-lookup"><span data-stu-id="f85eb-107">Windows MDM Security settings</span></span>
- <span data-ttu-id="f85eb-108">Microsoft zaštitnik za bezbednost krajnje tačke</span><span class="sxs-lookup"><span data-stu-id="f85eb-108">Microsoft Defender for EndPoint Security</span></span>
- <span data-ttu-id="f85eb-109">Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="f85eb-109">Microsoft Edge</span></span>

<span data-ttu-id="f85eb-110">Svaka osnovna podataka se ažurira periodično i objavljuje u inkrementalnim verzijama.</span><span class="sxs-lookup"><span data-stu-id="f85eb-110">Each of the baselines are updated periodically and released in incremental versions.</span></span> <span data-ttu-id="f85eb-111">Svaka verzija dodaje ili uklanja postavke iz prethodne verzije kako bi obezbedila da osnovna linija ispunjava trenutna uputstva.</span><span class="sxs-lookup"><span data-stu-id="f85eb-111">Each version adds and or removes settings from the previous version to ensure that the baseline meets current guidance.</span></span> <span data-ttu-id="f85eb-112">Konzola osnovnih podataka bezbednosti u bezbednosti krajnje tačke omogućava poređenje različitih verzija tako što menja verzije u vidljive verzije.</span><span class="sxs-lookup"><span data-stu-id="f85eb-112">The Security baselines console in Endpoint Security allows different versions to be compared by making the changes from version to version visible.</span></span>

<span data-ttu-id="f85eb-113">Uputstva o tome kako da na najefikasnije promenite koja je verzija osnovne linije primenjena, pogledajte članak Upravljanje profilima osnovnih linija bezbednosti [u aplikaciji Microsoft Intune.](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure)</span><span class="sxs-lookup"><span data-stu-id="f85eb-113">For guidance on how to most effectively change which version of baseline is deployed, see [Manage security baseline profiles in Microsoft Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure).</span></span>

<span data-ttu-id="f85eb-114">Nakon primene osnovne linije bezbednosti možete da nadgledate stanje primene i pregledate postavke na osnovu uređaja.</span><span class="sxs-lookup"><span data-stu-id="f85eb-114">After deploying a security baseline, you can monitor the state of deployment and review settings on a device-by-device basis.</span></span>

<span data-ttu-id="f85eb-115">**Napomogućeno:** Može biti vremena da se podaci izveštavanja za osnovne podatke pojave od do 24 časa od početne primene na uređaju i do 6 časova za buduće ispravke.</span><span class="sxs-lookup"><span data-stu-id="f85eb-115">**Note:** The reporting data for baselines may take up to 24 hours to appear from the initial deployment to a device and up to 6 hours for further updates.</span></span> 

<span data-ttu-id="f85eb-116">Najčešći uzrok postavke osnovne linije koja se ne primenjuje je zato što se ista postavka koristi na drugom profilu.</span><span class="sxs-lookup"><span data-stu-id="f85eb-116">The most common cause of a baseline setting not applying is because the same setting being used in a different profile.</span></span> <span data-ttu-id="f85eb-117">Ovaj scenario može da se istraži za određeni uređaj tako što će izabrati taj uređaj u okviru statusa uređaja profila osnovne linije bezbednosti.</span><span class="sxs-lookup"><span data-stu-id="f85eb-117">This scenario can be investigated for specific device by selecting that device from within the Device Status node of the Security Baseline profile.</span></span> <span data-ttu-id="f85eb-118">Više detalja ćete videti u [temi Otklanjanje neusaglašenosti za osnovne podatke o bezbednosti.](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines)</span><span class="sxs-lookup"><span data-stu-id="f85eb-118">For details, see [Resolve conflicts for security baselines](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines).</span></span>