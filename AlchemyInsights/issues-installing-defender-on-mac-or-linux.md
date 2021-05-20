---
title: Problemi sa instaliranjem programa Microsoft Zaštitnik na Mac ili Linux
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
ms.openlocfilehash: 39f180852fd0438597fa1ce665b2703fbc7b1aa4
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 05/19/2021
ms.locfileid: "52539694"
---
# <a name="issues-installing-microsoft-defender-on-mac-or-linux"></a><span data-ttu-id="00b59-102">Problemi sa instaliranjem programa Microsoft Zaštitnik na Mac ili Linux</span><span class="sxs-lookup"><span data-stu-id="00b59-102">Issues installing Microsoft Defender on Mac or Linux</span></span>

<span data-ttu-id="00b59-103">**Mac**</span><span class="sxs-lookup"><span data-stu-id="00b59-103">**Mac**</span></span>

- <span data-ttu-id="00b59-104">Uverite se da su sistemski zahtevi ispunjeni pre nego što ATP za Microsoft zaštitnik za Mac.</span><span class="sxs-lookup"><span data-stu-id="00b59-104">Ensure that system requirements are met before installing Microsoft Defender ATP for Mac.</span></span> <span data-ttu-id="00b59-105">Više informacija potražite u [članku Kako se instalira ATP za Microsoft zaštitnik za Mac.](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-mac#how-to-install-microsoft-defender-atp-for-mac)</span><span class="sxs-lookup"><span data-stu-id="00b59-105">For more info, see [How to install Microsoft Defender ATP for Mac](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-mac#how-to-install-microsoft-defender-atp-for-mac).</span></span>  
- <span data-ttu-id="00b59-106">Pregledajte informacije u datoteci: "/Biblioteka/Logs/Microsoft/mdatp/install.log".</span><span class="sxs-lookup"><span data-stu-id="00b59-106">Review the information in the file: "/Library/Logs/Microsoft/mdatp/install.log".</span></span>

<span data-ttu-id="00b59-107">**Linux**</span><span class="sxs-lookup"><span data-stu-id="00b59-107">**Linux**</span></span>

- <span data-ttu-id="00b59-108">Uverite se da su sistemski zahtevi ispunjeni pre nego što ATP za Microsoft zaštitnik za Linux.</span><span class="sxs-lookup"><span data-stu-id="00b59-108">Ensure that system requirements are met before installing Microsoft Defender ATP for Linux.</span></span> <span data-ttu-id="00b59-109">Više informacija potražite u [članku Instaliranje MDATP-a za Linux.](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements)</span><span class="sxs-lookup"><span data-stu-id="00b59-109">For more info, see [How to install MDATP for Linux](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements).</span></span> 
- <span data-ttu-id="00b59-110">Da biste potvrdili da je usluga MDATP pokrenuta, pogledajte tj. [Instalacija nije uspela.](/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#installation-failed)</span><span class="sxs-lookup"><span data-stu-id="00b59-110">To verify that MDATP service is running, see [Installation failed](/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#installation-failed).</span></span>  
    <span data-ttu-id="00b59-111">Da biste rešili probleme i rešili probleme ako usluga nije pokrenuta, pogledajte korake za rešavanje problema ako nije pokrenuta [u mdatp usluzi.](/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#steps-to-troubleshoot-if-mdatp-service-isnt-running)</span><span class="sxs-lookup"><span data-stu-id="00b59-111">To troubleshoot and resolve issues if the service is not running, see [Steps to troubleshoot if mdatp service isn't running](/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#steps-to-troubleshoot-if-mdatp-service-isnt-running).</span></span>
- <span data-ttu-id="00b59-112">Korake za proveru konfiguracije klijenta, koja proverava zdravlje proizvoda i testiranje otkrivanja u EICAR tekstualnoj datoteci, pogledajte konfiguraciju [klijenta.](/windows/security/threat-protection/microsoft-defender-atp/linux-install-manually#client-configuration)</span><span class="sxs-lookup"><span data-stu-id="00b59-112">For steps to check the client configuration, which verifies the health of the product, and to run a detection test on the EICAR text file, see [Client configuration](/windows/security/threat-protection/microsoft-defender-atp/linux-install-manually#client-configuration).</span></span>  

    <span data-ttu-id="00b59-113">**Napomišite** Listu podržanih sistema datoteka za aktivnost pristupa možete da vidite u ATP za Microsoft zaštitnik [za Linux.](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements)</span><span class="sxs-lookup"><span data-stu-id="00b59-113">**Note** For a list of supported file systems for on-access activity, see [Microsoft Defender ATP for Linux](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements).</span></span>