---
title: Problemi sa mašinama
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6023"
- "9002913"
ms.openlocfilehash: 19b516dc21472e2c80a8b9046f802b329d15e4d6
ms.sourcegitcommit: 45c2aaeee58c0be466b76c7f0cd71e796d3c8f76
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 07/15/2020
ms.locfileid: "45141659"
---
# <a name="issues-with-onboarding-machines"></a><span data-ttu-id="654d5-102">Problemi sa mašinama</span><span class="sxs-lookup"><span data-stu-id="654d5-102">Issues with onboarding machines</span></span>

<span data-ttu-id="654d5-103">Možda imate problema sa mašinama za uslugu "MDATP".</span><span class="sxs-lookup"><span data-stu-id="654d5-103">You might have issues with onboarding machines to MDATP service.</span></span> <span data-ttu-id="654d5-104">Ako možete da pristupite računaru krajnjeg korisnika, sledite ove korake:</span><span class="sxs-lookup"><span data-stu-id="654d5-104">If you can access the end-user machine, follow these steps:</span></span>

1. <span data-ttu-id="654d5-105">Preuzmite dijagnostičku alatku [analizator veze sa klijentom](https://aka.ms/mdatpanalyzer) .</span><span class="sxs-lookup"><span data-stu-id="654d5-105">Download the [Client Connectivity Analyzer](https://aka.ms/mdatpanalyzer) diagnostic tool.</span></span>
2. <span data-ttu-id="654d5-106">Izdvojite i pokrenite MDATPAnalyzer. cmd.</span><span class="sxs-lookup"><span data-stu-id="654d5-106">Extract and run MDATPAnalyzer.cmd.</span></span>
3. <span data-ttu-id="654d5-107">Pronađite evidenciju dijagnostike u fascikli pod nazivom Mdatpclientanalizator Zers, istu fasciklu u kojoj je preuzeta alatka za analizator.</span><span class="sxs-lookup"><span data-stu-id="654d5-107">Locate the diagnostic log in the folder called MDATPClientAnalyzerResult, the same folder where the Analyzer tool is downloaded.</span></span>
4. <span data-ttu-id="654d5-108">Pregledajte datoteku evidencije, MDATPClientAnalyzer.txt, da biste pronašli probleme sa mogućnošću povezivanja ili proxy postavki za Internet.</span><span class="sxs-lookup"><span data-stu-id="654d5-108">Review the log file, MDATPClientAnalyzer.txt, to find connectivity or internet proxy settings issues.</span></span>