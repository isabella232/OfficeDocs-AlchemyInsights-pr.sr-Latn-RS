---
title: Pravila za smanjenje površine napada
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
- "11228"
- "9005470"
ms.openlocfilehash: 99feaa5c3f35a0bb78b99f47ac2be88cf3e1b62a
ms.sourcegitcommit: 4b504650e11adb9894c37b6d8608b53f9d5fc13d
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 05/25/2021
ms.locfileid: "52676441"
---
# <a name="attack-surface-reduction-rules"></a><span data-ttu-id="f9555-102">Pravila za smanjenje površine napada</span><span class="sxs-lookup"><span data-stu-id="f9555-102">Attack surface reduction rules</span></span>

<span data-ttu-id="f9555-103">Isključivanje datoteka ili fascikli može ozbiljno da smanji zaštitu koju pružaju pravila za smanjenje površine napada.</span><span class="sxs-lookup"><span data-stu-id="f9555-103">Excluding files or folders can severely reduce the protection provided by attack surface reduction rules.</span></span> <span data-ttu-id="f9555-104">Datotekama koje je pravilo blokiralo dozvoljeno je da se pokrenu i nijedan izveštaj ili događaj se ne zapisuje.</span><span class="sxs-lookup"><span data-stu-id="f9555-104">Files that would have been blocked by a rule are allowed to run, and no report or event is recorded.</span></span> <span data-ttu-id="f9555-105">Izuzetke se primenjuju na sva pravila koja dozvoljavaju izuzetke.</span><span class="sxs-lookup"><span data-stu-id="f9555-105">An exclusion applies to all rules that allow exclusions.</span></span>

<span data-ttu-id="f9555-106">ASR izuvici koriste istu sintaksu kao Antivirusni program Microsoft zaštitnika izusci.</span><span class="sxs-lookup"><span data-stu-id="f9555-106">ASR exclusions use the same syntax as Microsoft Defender Antivirus exclusions.</span></span> <span data-ttu-id="f9555-107">Za detalje pogledajte Konfigurisanje i provera valjanosti izuzetka [za Antivirusni program Microsoft zaštitnika skeniranja.](/microsoft-365/security/defender-endpoint/configure-exclusions-microsoft-defender-antivirus)</span><span class="sxs-lookup"><span data-stu-id="f9555-107">For details, see [Configure and validate exclusions for Microsoft Defender Antivirus scans](/microsoft-365/security/defender-endpoint/configure-exclusions-microsoft-defender-antivirus).</span></span> <span data-ttu-id="f9555-108">Da biste izbegli probleme, [pregledajte uobičajene greške koje treba da izbegnete pri definisanju izuzetaka.](/microsoft-365/security/defender-endpoint/common-exclusion-mistakes-microsoft-defender-antivirus)</span><span class="sxs-lookup"><span data-stu-id="f9555-108">To avoid problems, review [Common mistakes to avoid when defining exclusions](/microsoft-365/security/defender-endpoint/common-exclusion-mistakes-microsoft-defender-antivirus).</span></span>

<span data-ttu-id="f9555-109">Ne podržavaju sva ASR pravila izuzetke.</span><span class="sxs-lookup"><span data-stu-id="f9555-109">Not all ASR rules support exclusions.</span></span> <span data-ttu-id="f9555-110">Da biste proverili da li pravilo podržava izuzetke, pogledajte tabelu Pravila za smanjenje površine [napada.](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules)</span><span class="sxs-lookup"><span data-stu-id="f9555-110">To validate if your rule supports exclusions, see the table [Attack surface reduction rules](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).</span></span>

## <a name="attack-surface-reduction-rules"></a><span data-ttu-id="f9555-111">Pravila za smanjenje površine napada</span><span class="sxs-lookup"><span data-stu-id="f9555-111">Attack surface reduction rules</span></span>

<span data-ttu-id="f9555-112">Površina napada u organizaciji obuhvata sva mesta na kojima napadač može da ugrozi organizacione uređaje ili mreže.</span><span class="sxs-lookup"><span data-stu-id="f9555-112">Your organization attack surface includes all the places where an attacker could compromise organization devices or networks.</span></span> <span data-ttu-id="f9555-113">Smanjivanje površine napada znači zaštita uređaja i mreže organizacije, što ostavlja napadače sa manje načina za vođenje napada.</span><span class="sxs-lookup"><span data-stu-id="f9555-113">Reducing your attack surface means protecting the organization devices and network, which leaves attackers with fewer ways to perform attacks.</span></span> <span data-ttu-id="f9555-114">Konfigurisanje pravila za smanjenje površine napada u Programu Microsoft zaštitnik za krajnju tačku može pomoći.</span><span class="sxs-lookup"><span data-stu-id="f9555-114">Configuring attack surface reduction rules in Microsoft Defender for Endpoint can help.</span></span>

<span data-ttu-id="f9555-115">Za više informacija pogledajte:</span><span class="sxs-lookup"><span data-stu-id="f9555-115">For more information, see:</span></span>

- [<span data-ttu-id="f9555-116">Mapiranje GUID-a ASR pravila za ime</span><span class="sxs-lookup"><span data-stu-id="f9555-116">Map ASR rule GUID to name</span></span>](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules)
- <span data-ttu-id="f9555-117">Zahtevi za ASR pravila:</span><span class="sxs-lookup"><span data-stu-id="f9555-117">ASR rules requirements:</span></span>
    - [<span data-ttu-id="f9555-118">Windows 10 Pro, verzija 1709 ili novija</span><span class="sxs-lookup"><span data-stu-id="f9555-118">Windows 10 Pro, version 1709 or later</span></span>](/windows/whats-new/whats-new-windows-10-version-1709)
    - [<span data-ttu-id="f9555-119">Windows 10 Enterprise, verzija 1709 ili novija</span><span class="sxs-lookup"><span data-stu-id="f9555-119">Windows 10 Enterprise, version 1709 or later</span></span>](/windows/whats-new/whats-new-windows-10-version-1709)
    - [<span data-ttu-id="f9555-120">Windows Server, verzija 1803 (polugodišnji kanal) ili novija</span><span class="sxs-lookup"><span data-stu-id="f9555-120">Windows Server, version 1803 (Semi-Annual Channel) or later</span></span>](/windows-server/get-started/whats-new-in-windows-server-1803)

## <a name="identify-the-correct-exclusion-to-apply"></a><span data-ttu-id="f9555-121">Identifikovanje odgovarajućeg izuzetka za primenu</span><span class="sxs-lookup"><span data-stu-id="f9555-121">Identify the correct exclusion to apply</span></span>

1. <span data-ttu-id="f9555-122">Potražite ID događaja 1121 ili 1122 u Microsoft-Windows-Windows zaštitnik/Operational evidenciji.</span><span class="sxs-lookup"><span data-stu-id="f9555-122">Look for eventID 1121 or 1122 in the Microsoft-Windows-Windows Defender/Operational log.</span></span>

1. <span data-ttu-id="f9555-123">Procenite scenario blokiranja i kontekst i potvrdite da ovaj scenario treba da se deblokira.</span><span class="sxs-lookup"><span data-stu-id="f9555-123">Evaluate the block scenario and context and confirm that this scenario needs to be unblocked.</span></span>

1. <span data-ttu-id="f9555-124">Pročitajte vrednost Putanja u detaljima događaja, što je vrednost koja definiše izuzetak.</span><span class="sxs-lookup"><span data-stu-id="f9555-124">Read the Path value in the event details, which is the value that defines the exclusion.</span></span>
    - <span data-ttu-id="f9555-125">Učinite izuzetke što je moguće strogim.</span><span class="sxs-lookup"><span data-stu-id="f9555-125">Make the exclusion as strict as possible.</span></span>
    - <span data-ttu-id="f9555-126">Primenite džoker znak tamo gde je potrebno (na primer, zamenite promenljivu Korisnik).</span><span class="sxs-lookup"><span data-stu-id="f9555-126">Apply a wildcard where needed (for example, replace User variable).</span></span>

1. <span data-ttu-id="f9555-127">Primenite izuzetak u skladu sa potrebama za primenom.</span><span class="sxs-lookup"><span data-stu-id="f9555-127">Apply the exclusion according to your deployment needs.</span></span> <span data-ttu-id="f9555-128">Za detalje pogledajte Prilagođavanje [pravila za smanjenje površine napada.](/microsoft-365/security/defender-endpoint/customize-attack-surface-reduction)</span><span class="sxs-lookup"><span data-stu-id="f9555-128">For details, see [Customize attack surface reduction rules](/microsoft-365/security/defender-endpoint/customize-attack-surface-reduction).</span></span>

## <a name="exclusion-is-not-honored"></a><span data-ttu-id="f9555-129">Izuvišnost se ne poštuje</span><span class="sxs-lookup"><span data-stu-id="f9555-129">Exclusion is not honored</span></span>

1. <span data-ttu-id="f9555-130">Utvrdite da li pravila podržavaju izuzetke.</span><span class="sxs-lookup"><span data-stu-id="f9555-130">Determine whether the rule support exclusions.</span></span> <span data-ttu-id="f9555-131">Za detalje pogledajte pravila [za smanjenje površine napada.](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules)</span><span class="sxs-lookup"><span data-stu-id="f9555-131">For details, see [Attack surface reduction rules](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).</span></span>

1. <span data-ttu-id="f9555-132">Pregledajte primenjene izuzetke i verifikujte sa podacima o događaju da biste unosili pogrešno protumačene džoker znakove.</span><span class="sxs-lookup"><span data-stu-id="f9555-132">Review the exclusions applied and verify with the event data for typos or misinterpreted wildcards.</span></span> <span data-ttu-id="f9555-133">Više informacija potražite u [članku Podržani tipovi izuzetka](/microsoft-365/security/defender-endpoint/mac-exclusions#supported-exclusion-types)</span><span class="sxs-lookup"><span data-stu-id="f9555-133">For more info, see [Supported exclusion types](/microsoft-365/security/defender-endpoint/mac-exclusions#supported-exclusion-types)</span></span>

1. <span data-ttu-id="f9555-134">ako je uticaj pravila previsoko, razmotrite premeštanje pravila (nazad) u režim nadzora radi dalje provere valjanosti.</span><span class="sxs-lookup"><span data-stu-id="f9555-134">if the impact of the rule it too high, consider moving the rule (back) to Audit mode to perform further validation.</span></span> <span data-ttu-id="f9555-135">Detalje možete da vidite u [članku Testiranje načina na koji funkcije Microsoft zaštitka za krajnje tačke rade u režimu nadzora.](/microsoft-365/security/defender-endpoint/audit-windows-defender)</span><span class="sxs-lookup"><span data-stu-id="f9555-135">For details, see [Test how Microsoft Defender for Endpoint features work in audit mode](/microsoft-365/security/defender-endpoint/audit-windows-defender).</span></span>

1. <span data-ttu-id="f9555-136">Prikupite podatke podrške da biste otvorili predmet podrške pomoću ove komande:</span><span class="sxs-lookup"><span data-stu-id="f9555-136">Collect support data to open a support case by using this command:</span></span>
    
   <span data-ttu-id="f9555-137">\*\* MDEClientAnalyzer.cmd -v\*\*</span><span class="sxs-lookup"><span data-stu-id="f9555-137">\*\* MDEClientAnalyzer.cmd -v\*\*</span></span>

    <span data-ttu-id="f9555-138">Više informacija potražite u [članku Problemi sa mašinama za ulaženje u Microsoft zaštitnik za krajnje tačke.](issues-with-onboarding-machines.md)</span><span class="sxs-lookup"><span data-stu-id="f9555-138">For more information, see [Issues with onboarding machines to Microsoft Defender for Endpoints](issues-with-onboarding-machines.md).</span></span>
