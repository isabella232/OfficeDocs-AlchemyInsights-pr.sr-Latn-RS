---
title: Primena Win32 aplikacije za primenu
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6446"
- "6700004"
ms.openlocfilehash: 5ccbf37bd3f06da2f8c3955d87e449ea58caab1c
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 10/06/2020
ms.locfileid: "48461992"
---
# <a name="intune-win32-app-deployment"></a><span data-ttu-id="1a900-102">Primena Win32 aplikacije za primenu</span><span class="sxs-lookup"><span data-stu-id="1a900-102">Intune Win32 app deployment</span></span>

<span data-ttu-id="1a900-103">Microsoft Intune omogućava Win32 aplikacijama, uključujući ali nije ograničeno na MSI i. EXE treba da bude raspoređena na Windows 10 uređaje.</span><span class="sxs-lookup"><span data-stu-id="1a900-103">Microsoft Intune allows Win32 applications, including but not limited to MSI and .EXE’s to be deployed to Windows 10 devices.</span></span> <span data-ttu-id="1a900-104">Korišćenje mehanizma za primenu zahteva proširenje Intune (IME) koje će biti na ciljnom uređaju.</span><span class="sxs-lookup"><span data-stu-id="1a900-104">The deployment mechanism used requires the Intune Management Extension (IME) to be present on the target device.</span></span> <span data-ttu-id="1a900-105">IME će se automatski instalirati kao rezultat automatskog usmeravanje ili Win32 primene aplikacije na korisnika/device.</span><span class="sxs-lookup"><span data-stu-id="1a900-105">The IME will be installed automatically as a result of targeting a powershell script or win32 application deployment to a user / device.</span></span>

<span data-ttu-id="1a900-106">Postoji i niz preduslova koji moraju da se ispune da bi se primenili Win32 aplikacije koje spadaju:</span><span class="sxs-lookup"><span data-stu-id="1a900-106">There are also a set of pre-requisites which must be met in order to deploy Win32 apps which include:</span></span>

- <span data-ttu-id="1a900-107">Podržane platforme: Windows 10 verzija 1607 ili novije verzije (Enterprise, Pro i obrazovni verzije).</span><span class="sxs-lookup"><span data-stu-id="1a900-107">Supported platforms: Windows 10 version 1607 or later (Enterprise, Pro, and Education versions).</span></span>
- <span data-ttu-id="1a900-108">Podržana arhitektura: x86 i x64.</span><span class="sxs-lookup"><span data-stu-id="1a900-108">Supported architecture: x86 and x64.</span></span>
- <span data-ttu-id="1a900-109">Upravljanje uređajima: AAD se pridružio i automatski upisan (uključujući hibridne domene pridruženu i grupne smernice grupe).</span><span class="sxs-lookup"><span data-stu-id="1a900-109">Device Management: AAD joined and auto-enrolled (including hybrid domain joined and group policy auto-enrolled).</span></span>
- <span data-ttu-id="1a900-110">Format paketa aplikacije:. IT **datoteka koju**  je pripremila [Microsoft Win32 alatka za pripremu sadržaja](https://docs.microsoft.com/mem/intune/apps/apps-win32-prepare).</span><span class="sxs-lookup"><span data-stu-id="1a900-110">Application Package format: .**intunewin**  file prepared by the [Microsoft Win32 content Prep tool](https://docs.microsoft.com/mem/intune/apps/apps-win32-prepare).</span></span>
- <span data-ttu-id="1a900-111">Vanje</span><span class="sxs-lookup"><span data-stu-id="1a900-111">Limitations:</span></span>
    - <span data-ttu-id="1a900-112">Maksimalna veličina: 8 GB.</span><span class="sxs-lookup"><span data-stu-id="1a900-112">Maximum size: 8GB.</span></span>
    - <span data-ttu-id="1a900-113">Nepodržana arhitektura: oružje.</span><span class="sxs-lookup"><span data-stu-id="1a900-113">Unsupported architecture: ARMs.</span></span>

<span data-ttu-id="1a900-114">Pregledajte stavku "[Dodavanje, dodela i nadgledanje Win32 aplikacije u programu Microsoft Intune](https://docs.microsoft.com/mem/intune/apps/apps-win32-add)" za informacije koje se tiču tih koraka.</span><span class="sxs-lookup"><span data-stu-id="1a900-114">Review the doc "[Add, assign, and monitor a Win32 app in Microsoft Intune](https://docs.microsoft.com/mem/intune/apps/apps-win32-add)" for information related to those steps.</span></span>

<span data-ttu-id="1a900-115">Detalji o rešavanju problema sa primenom aplikacije u operativnom sistemu Windows uključujući Win32 aplikacije mogu se redigovati u sledećim dokumentima</span><span class="sxs-lookup"><span data-stu-id="1a900-115">Details on troubleshooting application deployment on Windows including Win32 apps can be reviewed in the following documents</span></span>

- [<span data-ttu-id="1a900-116">Rešavanje problema sa instalacijom aplikacija</span><span class="sxs-lookup"><span data-stu-id="1a900-116">Troubleshoot App Installation issues</span></span>](https://docs.microsoft.com/mem/intune/apps/troubleshoot-app-install)  
- [<span data-ttu-id="1a900-117">Rešavanje problema sa Win32 aplikacijama</span><span class="sxs-lookup"><span data-stu-id="1a900-117">Troubleshoot Win32 Apps</span></span>](https://docs.microsoft.com/mem/intune/apps/apps-win32-troubleshoot)