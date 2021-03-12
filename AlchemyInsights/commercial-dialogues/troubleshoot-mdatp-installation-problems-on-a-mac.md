---
title: Rešavanje problema sa programom MDATP instalacija na Mac računaru
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
ms.openlocfilehash: 4b03361666f950a2010e4c4d8e78d156438d9e90
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/11/2021
ms.locfileid: "50749770"
---
# <a name="troubleshoot-mdatp-installation-problems-on-a-mac"></a><span data-ttu-id="b33e2-102">Rešavanje problema sa programom MDATP instalacija na Mac računaru</span><span class="sxs-lookup"><span data-stu-id="b33e2-102">Troubleshoot MDATP installation problems on a Mac</span></span>

<span data-ttu-id="b33e2-103">Ako Ručno instaliranje ne uspe, **stranica čarobnjaka** za instalaciju prikazuje sledeću grešku:</span><span class="sxs-lookup"><span data-stu-id="b33e2-103">If manual installation fails, the **Summary** page of the installation wizard shows the following error:</span></span>

<span data-ttu-id="b33e2-104">"Došlo je do greške tokom instalacije.</span><span class="sxs-lookup"><span data-stu-id="b33e2-104">"An error occurred during installation.</span></span> <span data-ttu-id="b33e2-105">Instalacioni program je naišao na grešku koja je izazvala otkazivanje instalacije.</span><span class="sxs-lookup"><span data-stu-id="b33e2-105">The Installer encountered an error that caused the installation to fail.</span></span> <span data-ttu-id="b33e2-106">Obratite se proizvođaču softvera za pomoć. "</span><span class="sxs-lookup"><span data-stu-id="b33e2-106">Contact the software manufacturer for assistance."</span></span>

<span data-ttu-id="b33e2-107">Za primena MDM-a, na stranici se prikazuje i Opšta greška.</span><span class="sxs-lookup"><span data-stu-id="b33e2-107">For MDM deployments, the page shows a generic installation failure, too.</span></span>

<span data-ttu-id="b33e2-108">Iako ne prikazujemo tačne greške za krajnji korisnik, zadržavamo datoteku evidencije sa napretkom instalacije, u **/Biblioteary/Logs/Microsoft/mdatp/Install.log**.</span><span class="sxs-lookup"><span data-stu-id="b33e2-108">Although we don't display exact errors to end users, we keep a log file with installation progress, in **/Library/Logs/Microsoft/mdatp/install.log**.</span></span> <span data-ttu-id="b33e2-109">Svaka sesija instalacije se dodaje na ovu datoteku evidencije.</span><span class="sxs-lookup"><span data-stu-id="b33e2-109">Each installation session appends to this log file.</span></span> <span data-ttu-id="b33e2-110">Da biste mogli da izvezete samo poslednju sesiju instalacije, koristite ih `sed` .</span><span class="sxs-lookup"><span data-stu-id="b33e2-110">To output the last installation session only, use `sed`.</span></span>

<span data-ttu-id="b33e2-111">Da biste saznali više, pogledajte članak [Rešavanje problema sa instalacijom za ATP za Mac Microsoft Defender](https://go.microsoft.com/fwlink/?linkid=2144615).</span><span class="sxs-lookup"><span data-stu-id="b33e2-111">To learn more, see [Troubleshoot installation issues for Microsoft Defender ATP for Mac](https://go.microsoft.com/fwlink/?linkid=2144615).</span></span>
