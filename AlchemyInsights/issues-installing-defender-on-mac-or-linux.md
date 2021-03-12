---
title: Problemi pri instaliranju programa Microsoft Defender na Mac ili Linux
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
- "6028"
- "9001222"
ms.openlocfilehash: a8d5ad2246b9b83e1e0a4d5be4dd8bb41c16e734
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "50713844"
---
# <a name="issues-installing-microsoft-defender-on-mac-or-linux"></a><span data-ttu-id="ff023-102">Problemi pri instaliranju programa Microsoft Defender na Mac ili Linux</span><span class="sxs-lookup"><span data-stu-id="ff023-102">Issues installing Microsoft Defender on Mac or Linux</span></span>

<span data-ttu-id="ff023-103">**Mac**</span><span class="sxs-lookup"><span data-stu-id="ff023-103">**Mac**</span></span>

- <span data-ttu-id="ff023-104">Uverite se da su sistemski zahtevi ispunjeni pre instaliranja ATP programa Microsoft Defender za Mac.</span><span class="sxs-lookup"><span data-stu-id="ff023-104">Ensure that system requirements are met before installing Microsoft Defender ATP for Mac.</span></span> <span data-ttu-id="ff023-105">Više informacija potražite u članku [Kako da instalirate ATP za Microsoft Defender za Mac](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-mac#how-to-install-microsoft-defender-atp-for-mac).</span><span class="sxs-lookup"><span data-stu-id="ff023-105">For more info, see [How to install Microsoft Defender ATP for Mac](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-mac#how-to-install-microsoft-defender-atp-for-mac).</span></span>  
- <span data-ttu-id="ff023-106">Pregledajte informacije u datoteci: "/Biblioteary/Logs/Microsoft/mdatp/Install.log".</span><span class="sxs-lookup"><span data-stu-id="ff023-106">Review the information in the file: "/Library/Logs/Microsoft/mdatp/install.log".</span></span>

<span data-ttu-id="ff023-107">**XA**</span><span class="sxs-lookup"><span data-stu-id="ff023-107">**Linux**</span></span>

- <span data-ttu-id="ff023-108">Uverite se da su sistemski zahtevi ispunjeni pre instaliranja ATP programa Microsoft Defender za Linux.</span><span class="sxs-lookup"><span data-stu-id="ff023-108">Ensure that system requirements are met before installing Microsoft Defender ATP for Linux.</span></span> <span data-ttu-id="ff023-109">Više informacija potražite u članku [Kako da instalirate ATP za Microsoft Defender za Linux](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements).</span><span class="sxs-lookup"><span data-stu-id="ff023-109">For more info, see [How to install Microsoft Defender ATP for Linux](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements).</span></span> 
- <span data-ttu-id="ff023-110">Da biste potvrdili da je usluga MDATP pokrenuta, pogledajte članak [nije uspelo](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#installation-failed).</span><span class="sxs-lookup"><span data-stu-id="ff023-110">To verify that MDATP service is running, see [Installation failed](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#installation-failed).</span></span>  
    <span data-ttu-id="ff023-111">Da biste rešili probleme ako usluga nije pokrenuta, pogledajte članak [koraci za rešavanje problema sa uslugom mdatp](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#steps-to-troubleshoot-if-mdatp-service-isnt-running).</span><span class="sxs-lookup"><span data-stu-id="ff023-111">To troubleshoot and resolve issues if the service is not running, see [Steps to troubleshoot if mdatp service isn't running](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#steps-to-troubleshoot-if-mdatp-service-isnt-running).</span></span>
- <span data-ttu-id="ff023-112">Da biste proverili konfiguraciju klijenta, koja potvrđuje zdravlje proizvoda i da biste pokrenuli test otkrivanja na EKAR tekstualnu datoteku, pogledajte članak [Konfiguracija klijenta](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-install-manually#client-configuration).</span><span class="sxs-lookup"><span data-stu-id="ff023-112">For steps to check the client configuration, which verifies the health of the product, and to run a detection test on the EICAR text file, see [Client configuration](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-install-manually#client-configuration).</span></span>  

    <span data-ttu-id="ff023-113">**Napomena** Listu podržanih sistema datoteka za pristup za pristup potražite u članku [ATP za Microsoft Defender za Linux](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements).</span><span class="sxs-lookup"><span data-stu-id="ff023-113">**Note** For a list of supported file systems for on-access activity, see [Microsoft Defender ATP for Linux](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements).</span></span>