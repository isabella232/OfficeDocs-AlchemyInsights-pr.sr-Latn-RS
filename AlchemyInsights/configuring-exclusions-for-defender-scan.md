---
title: Konfigurisanje izuzetaka za skeniranje ATP za Microsoft zaštitnik skeniranje
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6027"
- "9001464"
ms.openlocfilehash: 5eb18f4133aca93c1506f4975c8d0567bede8d57
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 05/19/2021
ms.locfileid: "52543699"
---
# <a name="configuring-exclusions-for-microsoft-defender-atp-scan"></a><span data-ttu-id="930a6-102">Konfigurisanje izuzetaka za skeniranje ATP za Microsoft zaštitnik skeniranje</span><span class="sxs-lookup"><span data-stu-id="930a6-102">Configuring exclusions for Microsoft Defender ATP scan</span></span>

<span data-ttu-id="930a6-103">Određene oznake tipa datoteke i lokacije fascikli obično možete da isključite iz ATP za Microsoft zaštitnik skeniranja.</span><span class="sxs-lookup"><span data-stu-id="930a6-103">In general, you can exclude certain file extensions and folder locations from Microsoft Defender ATP scans.</span></span> <span data-ttu-id="930a6-104">Možete da konfigurišete i izuzetke za datoteke koje su otvorili određeni procesi.</span><span class="sxs-lookup"><span data-stu-id="930a6-104">You can also configure exclusions for files opened by certain processes.</span></span> <span data-ttu-id="930a6-105">Više informacija potražite u članku Konfigurisanje i provera valjanosti izuzetka na osnovu [oznake](/windows/security/threat-protection/microsoft-defender-antivirus/configure-extension-file-exclusions-microsoft-defender-antivirus) tipa datoteke i lokacije fascikle i Konfigurisanje izuzetka za datoteke otvorene pomoću [procesa.](/windows/security/threat-protection/microsoft-defender-antivirus/configure-process-opened-file-exclusions-microsoft-defender-antivirus)</span><span class="sxs-lookup"><span data-stu-id="930a6-105">For more info, see, [Configure and validate exclusions based on file extension and folder location](/windows/security/threat-protection/microsoft-defender-antivirus/configure-extension-file-exclusions-microsoft-defender-antivirus) and [Configure exclusions for files opened by processes](/windows/security/threat-protection/microsoft-defender-antivirus/configure-process-opened-file-exclusions-microsoft-defender-antivirus) .</span></span>

<span data-ttu-id="930a6-106">Da biste konfigurisali izuzetke za **Windows Server 2016 i 2019,** pogledajte konfigurisanje Antivirusni program Microsoft zaštitnika izuzetak na [Windows serveru.](/windows/security/threat-protection/microsoft-defender-antivirus/configure-server-exclusions-microsoft-defender-antivirus)</span><span class="sxs-lookup"><span data-stu-id="930a6-106">To configure exclusions for  **Windows Server 2016 and 2019**, see [Configure Microsoft Defender Antivirus exclusions on Windows Server](/windows/security/threat-protection/microsoft-defender-antivirus/configure-server-exclusions-microsoft-defender-antivirus).</span></span>

<span data-ttu-id="930a6-107">**Mac**</span><span class="sxs-lookup"><span data-stu-id="930a6-107">**Mac**</span></span>

<span data-ttu-id="930a6-108">Detalje o podržanim tipovima izuzetaka i konfigurisanju liste izuzetaka za Mac, pogledajte podržani tipovi izuzetaka i Kako konfigurisati listu [](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#supported-exclusion-types) izuzetaka. [](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#how-to-configure-the-list-of-exclusions)</span><span class="sxs-lookup"><span data-stu-id="930a6-108">For details on supported exclusion types and configuring a list of exclusions for Mac, see [Supported exclusion types](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#supported-exclusion-types) and [How to configure the list of exclusions](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#how-to-configure-the-list-of-exclusions).</span></span>

<span data-ttu-id="930a6-109">**Napomišite** Takođe možete da proverite valjanost lista izuzetka pomoću EICAR probne datoteke.</span><span class="sxs-lookup"><span data-stu-id="930a6-109">**Note** You can also validate exclusions lists using the EICAR test file.</span></span> <span data-ttu-id="930a6-110">Više informacija potražite u članku Provera valjanosti lista izuzetka u [EICAR datoteci za testiranje.](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#validate-exclusions-lists-with-the-eicar-test-file)</span><span class="sxs-lookup"><span data-stu-id="930a6-110">For more info, see [Validate exclusions lists with the EICAR test file](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span></span> 

<span data-ttu-id="930a6-111">**Linux**</span><span class="sxs-lookup"><span data-stu-id="930a6-111">**Linux**</span></span>

<span data-ttu-id="930a6-112">Detalje o podržanim tipovima izuzetaka i konfigurisanju liste izuzetaka za Linux, pogledajte podržani tipovi izuzetaka i Konfigurisanje i provera valjanosti izuzetaka za [ATP za Microsoft zaštitnik linux.](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions) [](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#supported-exclusion-types)</span><span class="sxs-lookup"><span data-stu-id="930a6-112">For details on supported exclusion types and configuring a list of exclusions for Linux, see [Supported exclusion types](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#supported-exclusion-types) and [Configure and validate exclusions for Microsoft Defender ATP for Linux](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions).</span></span>

<span data-ttu-id="930a6-113">**Napomišite** Takođe možete da proverite valjanost lista izuzetka pomoću EICAR probne datoteke.</span><span class="sxs-lookup"><span data-stu-id="930a6-113">**Note** You can also validate exclusions lists using the EICAR test file.</span></span> <span data-ttu-id="930a6-114">Više informacija potražite u članku Provera valjanosti lista izuzetka u [EICAR datoteci za testiranje.](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#validate-exclusions-lists-with-the-eicar-test-file)</span><span class="sxs-lookup"><span data-stu-id="930a6-114">For more info, see [Validate exclusions lists with the EICAR test file](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span></span> 