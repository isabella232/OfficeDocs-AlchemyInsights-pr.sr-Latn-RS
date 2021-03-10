---
title: Daljinski rešite probleme sa sistemom Windows 10 uređajima na dodatnu zaštitu pretnje u usluzi Microsoft Defender
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 5473d090f6d4680f9a62f34f943ac6cea53b2079
ms.sourcegitcommit: 4883f1f89d4c6ca23161e9a43ff206ad21d4f09b
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/08/2021
ms.locfileid: "50694847"
---
# <a name="remotely-fix-problems-with-onboarding-windows-10-devices-to-microsoft-defender-advanced-threat-protection"></a><span data-ttu-id="a577e-102">Daljinski rešite probleme sa sistemom Windows 10 uređajima na dodatnu zaštitu pretnje u usluzi Microsoft Defender</span><span class="sxs-lookup"><span data-stu-id="a577e-102">Remotely fix problems with onboarding Windows 10 devices to Microsoft Defender Advanced Threat Protection</span></span>

<span data-ttu-id="a577e-103">Ako možete da pristupite udaljenom računaru, slijedite ove korake:</span><span class="sxs-lookup"><span data-stu-id="a577e-103">If you can access the remote computer, follow these steps:</span></span>

1. <span data-ttu-id="a577e-104">Preuzmite dijagnostičku alatku za [Povezivanje klijenata](https://go.microsoft.com/fwlink/?linkid=2143466) .</span><span class="sxs-lookup"><span data-stu-id="a577e-104">Download the [Client Connectivity Analyzer](https://go.microsoft.com/fwlink/?linkid=2143466) diagnostic tool.</span></span>
2. <span data-ttu-id="a577e-105">Izdvajanje i pokreće Mdatpanalycer. cmd.</span><span class="sxs-lookup"><span data-stu-id="a577e-105">Extract and run MDATPAnalyzer.cmd.</span></span>
3. <span data-ttu-id="a577e-106">Pronađite evidenciju dijagnostike u MDATPClientAnalyzerResult fascikli, koja je ista fascikla u kojoj je preuzeta alatka analitička.</span><span class="sxs-lookup"><span data-stu-id="a577e-106">Locate the diagnostic log in the MDATPClientAnalyzerResult folder, which is the same folder where the Analyzer tool was downloaded.</span></span>
4. <span data-ttu-id="a577e-107">Da biste pronašli probleme sa povezivanjem ili postavkama Internet proxy servera, pregledajte MDATPClientAnalyzer.txt datoteku evidencije.</span><span class="sxs-lookup"><span data-stu-id="a577e-107">To find issues with connectivity or Internet proxy settings, review the log file MDATPClientAnalyzer.txt.</span></span>

<span data-ttu-id="a577e-108">Da biste saznali više, pogledajte članak [problemi sa onboarnim mašinama](https://go.microsoft.com/fwlink/?linkid=2143634).</span><span class="sxs-lookup"><span data-stu-id="a577e-108">To learn more, see [Issues with onboarding machines](https://go.microsoft.com/fwlink/?linkid=2143634).</span></span>
