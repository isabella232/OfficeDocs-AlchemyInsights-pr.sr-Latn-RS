---
title: Endpoint Manager – odrednice bezbednosti
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
- "10064"
- "9003771"
ms.openlocfilehash: 36b480c7ed4715338fda056eafd69c511093e627
ms.sourcegitcommit: bef118c00aa397cd6d8941d403fe9cfa49dd8c73
ms.translationtype: HT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/30/2021
ms.locfileid: "51440907"
---
# <a name="endpoint-manager---security-baselines"></a><span data-ttu-id="c0833-102">Endpoint Manager – odrednice bezbednosti</span><span class="sxs-lookup"><span data-stu-id="c0833-102">EndPoint Manager - Security baselines</span></span>

<span data-ttu-id="c0833-103">Osnovne informacije o bezbednosti su unapred konfigurisane grupe postavki operativnog sistema Windows koje vam pomažu da primenite bezbednosne postavke koje preporučuju relevantni bezbednosni timovi.</span><span class="sxs-lookup"><span data-stu-id="c0833-103">Security baselines are pre-configured groups of Windows settings that help you apply the security settings recommended by the relevant security teams.</span></span> <span data-ttu-id="c0833-104">Ove odrednice mogu da se prilagode tako da isporuče samo postavke i vrednosti koje želite.</span><span class="sxs-lookup"><span data-stu-id="c0833-104">These baselines can be customized to deliver only the settings and values desired.</span></span> <span data-ttu-id="c0833-105">Više informacija o osnovnim informacijama o bezbednosti pogledajte u [Korišćenje osnovnih podataka o bezbednosti za konfigurisanje Windows 10 uređaja u Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines).</span><span class="sxs-lookup"><span data-stu-id="c0833-105">For more information about security baselines, see [Use security baselines to configure Windows 10 devices in Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines).</span></span>

<span data-ttu-id="c0833-106">Trenutno postoje odrednice za ove proizvode:</span><span class="sxs-lookup"><span data-stu-id="c0833-106">There are currently baselines for these products:</span></span>

- <span data-ttu-id="c0833-107">Windows MDM bezbednosne postavke</span><span class="sxs-lookup"><span data-stu-id="c0833-107">Windows MDM Security settings</span></span>
- <span data-ttu-id="c0833-108">Microsoft zaštitnik za EndPoint bezbednost</span><span class="sxs-lookup"><span data-stu-id="c0833-108">Microsoft Defender for EndPoint Security</span></span>
- <span data-ttu-id="c0833-109">Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="c0833-109">Microsoft Edge</span></span>

<span data-ttu-id="c0833-110">Svaka odrednica se periodično ažurira i objavljuje u inkrementalnim verzijama.</span><span class="sxs-lookup"><span data-stu-id="c0833-110">Each of the baselines are updated periodically and released in incremental versions.</span></span> <span data-ttu-id="c0833-111">Svaka verzija dodaje ili uklanja postavke iz prethodne verzije kako bi se obezbedilo da odrednica ispunjava trenutna uputstva.</span><span class="sxs-lookup"><span data-stu-id="c0833-111">Each version adds and or removes settings from the previous version to ensure that the baseline meets current guidance.</span></span> <span data-ttu-id="c0833-112">Konzola odrednica sigurnosti u programu Endpoint bezbednost omogućava upoređivanje različitih verzija čineći promene iz verzije u verziju vidljivim.</span><span class="sxs-lookup"><span data-stu-id="c0833-112">The Security baselines console in Endpoint Security allows different versions to be compared by making the changes from version to version visible.</span></span>

<span data-ttu-id="c0833-113">Uputstvo o tome kako da na najefikasniji način promenite koja se verzija odrednica primenjuje možete da vidite u članku [Upravljanje osnovnim profilima bezbednosti u aplikaciji Microsoft Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure).</span><span class="sxs-lookup"><span data-stu-id="c0833-113">For guidance on how to most effectively change which version of baseline is deployed, see [Manage security baseline profiles in Microsoft Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure).</span></span>

<span data-ttu-id="c0833-114">Nakon primene odrednica bezbednosti možete da pratite stanje primene i pregledate postavke od uređaja do uređaja.</span><span class="sxs-lookup"><span data-stu-id="c0833-114">After deploying a security baseline, you can monitor the state of deployment and review settings on a device-by-device basis.</span></span>

<span data-ttu-id="c0833-115">**Namena:** podaci o izveštavanju za odrednice mogu potrajati i do 24 sata da se pojave od početne primene na uređaju i do 6 sati za dalja ažuriranja.</span><span class="sxs-lookup"><span data-stu-id="c0833-115">**Note:** The reporting data for baselines may take up to 24 hours to appear from the initial deployment to a device and up to 6 hours for further updates.</span></span> 

<span data-ttu-id="c0833-116">Najčešći uzrok postavke odrednice koja se ne primenjuje jeste zato što se ista postavka koristi na drugom profilu.</span><span class="sxs-lookup"><span data-stu-id="c0833-116">The most common cause of a baseline setting not applying is because the same setting being used in a different profile.</span></span> <span data-ttu-id="c0833-117">Ovaj scenario se može istražiti za određeni uređaj tako što će izabrati taj uređaj u okviru statusa uređaja u okviru profila bezbednosne odrednice.</span><span class="sxs-lookup"><span data-stu-id="c0833-117">This scenario can be investigated for specific device by selecting that device from within the Device Status node of the Security Baseline profile.</span></span> <span data-ttu-id="c0833-118">Detalje možete da vidite u [Rešavanje neusaglašenosti za bezbednosne odrednice](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines).</span><span class="sxs-lookup"><span data-stu-id="c0833-118">For details, see [Resolve conflicts for security baselines](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines).</span></span>