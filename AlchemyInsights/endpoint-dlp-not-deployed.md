---
title: DLP krajnja tačka nije primenjena na uređaj korisnika
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/27/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11470"
- "9000292"
ms.openlocfilehash: 948835f5468b480536c176bfdf3b4eefb76b3bdb
ms.sourcegitcommit: c32233a1b7e6f1b07913d25f90189a58a8de2560
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 05/27/2021
ms.locfileid: "52731866"
---
# <a name="endpoint-dlp-not-deployed-to-users-device"></a><span data-ttu-id="c9ebc-102">DLP krajnja tačka nije primenjena na uređaj korisnika</span><span class="sxs-lookup"><span data-stu-id="c9ebc-102">Endpoint DLP not deployed to user's device</span></span>

<span data-ttu-id="c9ebc-103">Ako postavka sprečavanja gubitka podataka krajnje tačke (DLP) nije primenjena na uređaj korisnika, proverite da li ispunjavate ove zahteve:</span><span class="sxs-lookup"><span data-stu-id="c9ebc-103">If the Endpoint data loss prevention (DLP) setting has not applied to a user's device, confirm you meet these requirements:</span></span>

- <span data-ttu-id="c9ebc-104">Windows 10 x64 operativnog sistema 1809 ili novija, instalirana je na uređaju.</span><span class="sxs-lookup"><span data-stu-id="c9ebc-104">Windows 10 x64 build 1809 or later is installed on the device.</span></span>
- <span data-ttu-id="c9ebc-105">Instalirana je verzija klijenta za borbu protiv malvera 4.18.2009.7 ili novija.</span><span class="sxs-lookup"><span data-stu-id="c9ebc-105">Anti-malware client version 4.18.2009.7 or later is installed.</span></span>
- <span data-ttu-id="c9ebc-106">Uređaj je **jedan od** ovih:</span><span class="sxs-lookup"><span data-stu-id="c9ebc-106">The device is **one** of these:</span></span>
    
    - <span data-ttu-id="c9ebc-107">Azure Active Directory (Azure AD) pridružen</span><span class="sxs-lookup"><span data-stu-id="c9ebc-107">Azure Active Directory (Azure AD) joined</span></span>
    - <span data-ttu-id="c9ebc-108">Hibridni Azure AD pridružen</span><span class="sxs-lookup"><span data-stu-id="c9ebc-108">Hybrid Azure AD joined</span></span>
    - <span data-ttu-id="c9ebc-109">AAD registrovan</span><span class="sxs-lookup"><span data-stu-id="c9ebc-109">AAD registered</span></span>

- <span data-ttu-id="c9ebc-110">Da biste na primenili radnje smernica, proverite Chromium pregledač Microsoft Chromium Edge instaliran na uređaju krajnje tačke.</span><span class="sxs-lookup"><span data-stu-id="c9ebc-110">To enforce policy actions, make sure Microsoft Chromium Edge browser is installed on the endpoint device.</span></span>

<span data-ttu-id="c9ebc-111">Dodatne zahteve za primenu DLP krajnje tačke možete da dobijete u temi Prvi koraci uz sprečavanje [gubitka podataka krajnje tačke.](/microsoft-365/compliance/endpoint-dlp-getting-started#prepare-your-endpoints)</span><span class="sxs-lookup"><span data-stu-id="c9ebc-111">For additional requirements for deploying Endpoint DLP, see [Get started with Endpoint data loss prevention](/microsoft-365/compliance/endpoint-dlp-getting-started#prepare-your-endpoints).</span></span>