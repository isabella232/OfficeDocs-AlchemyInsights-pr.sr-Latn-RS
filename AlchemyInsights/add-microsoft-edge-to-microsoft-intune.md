---
title: Dodavanje Microsoft Edge aplikacije Microsoft Intune
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/10/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8240"
- "9004604"
ms.openlocfilehash: d56c65910d1c2170d3e0ce9676e913663701db96
ms.sourcegitcommit: 03378c78eadac5d950802dcbacc328bca3314032
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 02/10/2021
ms.locfileid: "50194574"
---
# <a name="add-microsoft-edge-to-microsoft-intune"></a><span data-ttu-id="d5471-102">Dodavanje Microsoft Edge aplikacije Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="d5471-102">Add Microsoft Edge to Microsoft Intune</span></span>

<span data-ttu-id="d5471-103">Da biste mogli da primenite, konfigurišete, pratite i zaštitite Microsoft Edge za Windows 10, prvo morate da ga dodate u Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="d5471-103">To be able to deploy, configure, monitor, and protect Microsoft Edge for Windows 10, you must first add it to Microsoft Intune.</span></span>

> [!IMPORTANT]
- <span data-ttu-id="d5471-104">Intune podržava Microsoft Edge 77 i novije verzije.</span><span class="sxs-lookup"><span data-stu-id="d5471-104">Intune supports Microsoft Edge 77 and later versions.</span></span>
- <span data-ttu-id="d5471-105">Intune će otkriti bilo koje postojeće instalacije Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="d5471-105">Intune will detect any pre-existing installations of Microsoft Edge.</span></span>
- <span data-ttu-id="d5471-106">Ako je Microsoft Edge instaliran u kontekstu korisnika, instalacija sistema će zameniti instalaciju u kontekstu korisnika.</span><span class="sxs-lookup"><span data-stu-id="d5471-106">If Microsoft Edge is installed in user context, a system installation will overwrite the installation in user context.</span></span>
- <span data-ttu-id="d5471-107">Ako se Microsoft Edge instalira u kontekstu sistema, pojaviće se uspešan instaliranje.</span><span class="sxs-lookup"><span data-stu-id="d5471-107">If Microsoft Edge is installed in system context, the installation success will be reported.</span></span>
- <span data-ttu-id="d5471-108">Unapred instalirana Microsoft Edge 77 i novije verzije, za sve kanale u kontekstu korisnika, biće zamenjena Microsoft Edge instaliranom u kontekstu sistema System.</span><span class="sxs-lookup"><span data-stu-id="d5471-108">Pre-installed Microsoft Edge 77 and later versions, for all channels in user context, will be overwritten with Microsoft Edge installed in system context.</span></span>

<span data-ttu-id="d5471-109">**Preduslovi**</span><span class="sxs-lookup"><span data-stu-id="d5471-109">**Prerequisite**</span></span>

<span data-ttu-id="d5471-110">Windows 10 verzija 1709 ili novije verzije</span><span class="sxs-lookup"><span data-stu-id="d5471-110">Windows 10 version 1709 or later versions</span></span>

<span data-ttu-id="d5471-111">**Koraci za Dodavanje ivice Intune**</span><span class="sxs-lookup"><span data-stu-id="d5471-111">**Steps to add Edge to Intune**</span></span>

1. <span data-ttu-id="d5471-112">[Konfigurišite aplikaciju u programu Intune](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span><span class="sxs-lookup"><span data-stu-id="d5471-112">[Configure the app in Intune](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>
2. <span data-ttu-id="d5471-113">[Konfigurisanje informacija o aplikaciji](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span><span class="sxs-lookup"><span data-stu-id="d5471-113">[Configure the app information](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>
3. <span data-ttu-id="d5471-114">[Konfigurišite postavke aplikacije](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span><span class="sxs-lookup"><span data-stu-id="d5471-114">[Configure the app settings](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>
4. <span data-ttu-id="d5471-115">[Izaberite oznake opsega (opcionalno)](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span><span class="sxs-lookup"><span data-stu-id="d5471-115">[Select the scope tags (optional)](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>
5. <span data-ttu-id="d5471-116">[Dodajte aplikaciju](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span><span class="sxs-lookup"><span data-stu-id="d5471-116">[Add the app](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>

<span data-ttu-id="d5471-117">Dodatne pomoći potražite u članku [Rešavanje problema](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span><span class="sxs-lookup"><span data-stu-id="d5471-117">For more help, see [Troubleshooting](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>




