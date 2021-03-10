---
title: Konfigurisanje i validacija isključivanja za MDATP na Linux mašini
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
ms.openlocfilehash: 4fad0a513f7c6d2f0337019488a4055c25e1650d
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/09/2021
ms.locfileid: "50696068"
---
# <a name="configure-and-validate-exclusions-for-mdatp-on-a-linux-machine"></a><span data-ttu-id="1a84c-102">Konfigurisanje i validacija isključivanja za MDATP na Linux mašini</span><span class="sxs-lookup"><span data-stu-id="1a84c-102">Configure and validate exclusions for MDATP on a Linux machine</span></span>

<span data-ttu-id="1a84c-103">Možete da isključite datoteke, fascikle, procese i datoteke koje su otvorene za procese iz usluge MDATP.</span><span class="sxs-lookup"><span data-stu-id="1a84c-103">You can exclude certain files, folders, processes, and process-opened files from MDATP scans.</span></span> <span data-ttu-id="1a84c-104">Isključivanja pomoći sprečavaju nepravilno otkrivanje softvera i datoteka jedinstvenih ili prilagođene organizaciji.</span><span class="sxs-lookup"><span data-stu-id="1a84c-104">Exclusions help prevent incorrect detection of software and files unique or customized to your organization.</span></span> <span data-ttu-id="1a84c-105">Isključenosti takođe pomažu da se umanjenje problema sa performansama izazove MDATP.</span><span class="sxs-lookup"><span data-stu-id="1a84c-105">Exclusions also help mitigate performance problems caused by MDATP.</span></span>

<span data-ttu-id="1a84c-106">Da biste saznali više, pogledajte članak [Konfigurisanje i validacija isključivanja za MDATP za Linux](https://go.microsoft.com/fwlink/?linkid=2144517).</span><span class="sxs-lookup"><span data-stu-id="1a84c-106">To learn more, see [Configure and validate exclusions for MDATP for Linux](https://go.microsoft.com/fwlink/?linkid=2144517).</span></span>

> [!IMPORTANT]
> <span data-ttu-id="1a84c-107">Isključivanja opisane u ovom članku ne primenjuju se na druge mogućnosti proizvoda MDATP za Linux, uključujući otkrivanje krajnje tačke i odgovor (EDR).</span><span class="sxs-lookup"><span data-stu-id="1a84c-107">The exclusions described in this article don't apply to other capabilities of MDATP for Linux, including endpoint detection and response (EDR).</span></span> <span data-ttu-id="1a84c-108">Datoteke koje isključavate koristeći metode opisane u ovom članku mogu i dalje da aktiviraju EDR obaveštenja i druge mogućnosti otkrivanja.</span><span class="sxs-lookup"><span data-stu-id="1a84c-108">Files that you exclude by using the methods described in this article can still trigger EDR alerts and other detection capabilities.</span></span>
