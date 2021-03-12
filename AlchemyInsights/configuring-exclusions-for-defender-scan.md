---
title: Konfigurisanje isključivanja za ATP sken Microsoft Defender
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
ms.openlocfilehash: 912e77b9b1a149fef373f2d0814fb2f0671a48c6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "50713904"
---
# <a name="configuring-exclusions-for-microsoft-defender-atp-scan"></a><span data-ttu-id="11304-102">Konfigurisanje isključivanja za ATP sken Microsoft Defender</span><span class="sxs-lookup"><span data-stu-id="11304-102">Configuring exclusions for Microsoft Defender ATP scan</span></span>

<span data-ttu-id="11304-103">Generalno, možete da isključite određene oznake tipa datoteke i lokacija fascikle iz ATP skeniranja Microsoft Defender.</span><span class="sxs-lookup"><span data-stu-id="11304-103">In general, you can exclude certain file extensions and folder locations from Microsoft Defender ATP scans.</span></span> <span data-ttu-id="11304-104">Možete i da konfigurišete isključenosti za datoteke koje su otvorene određenim procesima.</span><span class="sxs-lookup"><span data-stu-id="11304-104">You can also configure exclusions for files opened by certain processes.</span></span> <span data-ttu-id="11304-105">Više informacija potražite u članku [Konfigurisanje i validacije isključenja na osnovu oznake tipa datoteke i lokacije fascikle](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-extension-file-exclusions-microsoft-defender-antivirus) i [Konfigurisanje isključivanja za datoteke koje otvaraju procesi](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-process-opened-file-exclusions-microsoft-defender-antivirus) .</span><span class="sxs-lookup"><span data-stu-id="11304-105">For more info, see, [Configure and validate exclusions based on file extension and folder location](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-extension-file-exclusions-microsoft-defender-antivirus) and [Configure exclusions for files opened by processes](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-process-opened-file-exclusions-microsoft-defender-antivirus) .</span></span>

<span data-ttu-id="11304-106">Da biste konfigurisali isključivanja za  **Windows Server 2016 i 2019**, pogledajte članak [Konfigurisanje isključivanja antivirusnih isključenja Microsoft Defender na Windows serveru](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-server-exclusions-microsoft-defender-antivirus).</span><span class="sxs-lookup"><span data-stu-id="11304-106">To configure exclusions for  **Windows Server 2016 and 2019**, see [Configure Microsoft Defender Antivirus exclusions on Windows Server](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-server-exclusions-microsoft-defender-antivirus).</span></span>

<span data-ttu-id="11304-107">**Mac**</span><span class="sxs-lookup"><span data-stu-id="11304-107">**Mac**</span></span>

<span data-ttu-id="11304-108">Detalje o podržanim tipovima izuzetaka i konfigurisanju liste isključenosti za Mac potražite u članku [Podržani tipovi izuzetaka](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#supported-exclusion-types) i [Konfigurisanje liste isključenja](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#how-to-configure-the-list-of-exclusions).</span><span class="sxs-lookup"><span data-stu-id="11304-108">For details on supported exclusion types and configuring a list of exclusions for Mac, see [Supported exclusion types](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#supported-exclusion-types) and [How to configure the list of exclusions](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#how-to-configure-the-list-of-exclusions).</span></span>

<span data-ttu-id="11304-109">**Napomena** Možete i da proverite liste isključenja pomoću EKAR probne datoteke.</span><span class="sxs-lookup"><span data-stu-id="11304-109">**Note** You can also validate exclusions lists using the EICAR test file.</span></span> <span data-ttu-id="11304-110">Više informacija potražite u članku [Provera valjanosti isključive liste sa datotekom za testiranje ekar](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span><span class="sxs-lookup"><span data-stu-id="11304-110">For more info, see [Validate exclusions lists with the EICAR test file](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span></span> 

<span data-ttu-id="11304-111">**XA**</span><span class="sxs-lookup"><span data-stu-id="11304-111">**Linux**</span></span>

<span data-ttu-id="11304-112">Detalje o podržanim tipovima izuzetaka i konfigurisanju liste isključivanja za Linux potražite u članku [Podržani tipovi izuzetaka](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#supported-exclusion-types) i [Konfigurisanje i validacija isključenja za Microsoft Defender ATP za Linux](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions).</span><span class="sxs-lookup"><span data-stu-id="11304-112">For details on supported exclusion types and configuring a list of exclusions for Linux, see [Supported exclusion types](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#supported-exclusion-types) and [Configure and validate exclusions for Microsoft Defender ATP for Linux](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions).</span></span>

<span data-ttu-id="11304-113">**Napomena** Možete i da proverite liste isključenja pomoću EKAR probne datoteke.</span><span class="sxs-lookup"><span data-stu-id="11304-113">**Note** You can also validate exclusions lists using the EICAR test file.</span></span> <span data-ttu-id="11304-114">Više informacija potražite u članku [Provera valjanosti isključive liste sa datotekom za testiranje ekar](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span><span class="sxs-lookup"><span data-stu-id="11304-114">For more info, see [Validate exclusions lists with the EICAR test file](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span></span> 