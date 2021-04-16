---
title: Duplirani zapis uređaja u portalu
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001495"
- "4386"
ms.openlocfilehash: e6f477807823e68965ce966faf0a6f50f9472f3d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814530"
---
# <a name="duplicate-device-record-in-the-portal"></a><span data-ttu-id="d0889-102">Duplirani zapis uređaja u portalu</span><span class="sxs-lookup"><span data-stu-id="d0889-102">Duplicate device record in the portal</span></span>

<span data-ttu-id="d0889-103">Možda ćete videti 2 zapisa za uređaj na portalu ako uređaj ne prijavi tačno prijavljivanje statusa za saradnju na sajt upravljača konfigurisanja.</span><span class="sxs-lookup"><span data-stu-id="d0889-103">You may see 2 records for a device in the portal if the device does not correctly report the co-management status to the Configuration Manager site.</span></span> <span data-ttu-id="d0889-104">Da biste proverili status koordinatora uređaja, pregledajte  kolonu za uređaj u alatki "Upravljač konfigurisanja" u okviru Konzola za upravljanje.</span><span class="sxs-lookup"><span data-stu-id="d0889-104">To check the co-management status of a device, review the **Co-managed** column for the device in the Configuration Manager console.</span></span> <span data-ttu-id="d0889-105">Ako kolona nije vidljiva, možete da je dodate tako što ćete kliknuti desnim tasterom miša na bilo koje zaglavlja kolona i odabrati ga sa liste.</span><span class="sxs-lookup"><span data-stu-id="d0889-105">If the column is not visible, you may add it by right-clicking any of the column headers, and selecting it from the list.</span></span>

<span data-ttu-id="d0889-106">Zajednički kontrolisana vrednost mora da bude **Da**.</span><span class="sxs-lookup"><span data-stu-id="d0889-106">The Co-managed value must be **Yes**.</span></span> <span data-ttu-id="d0889-107">Ako je vrednost **Ne**, otvorite aplet za Menadžer konfigurisanja klijenta na uređaju klijenta i potvrdite izbor u polju za potvrdu **Saradništvo** na kartici Opšte.</span><span class="sxs-lookup"><span data-stu-id="d0889-107">If the value is **No**, open the Configuration Manager client applet on the client device and check the **Co-management** property in the General tab.</span></span>

- <span data-ttu-id="d0889-108">Ako je vrednost **omogućena**, to ukazuje na probleme sa komunikacijom klijenta uz management Point.</span><span class="sxs-lookup"><span data-stu-id="d0889-108">If the value is **Enabled**, this indicates problems with client communication with the Management Point.</span></span> <span data-ttu-id="d0889-109">Pregledajte **CcmMessaging. log** na uređaju da biste istražili potencijalne probleme sa povezivanjem.</span><span class="sxs-lookup"><span data-stu-id="d0889-109">Please review the **CcmMessaging.log** on the device to investigate potential connectivity issues.</span></span>

- <span data-ttu-id="d0889-110">Ako je vrednost **onemogućena**, a uređaj je upisan u Intune, uverite se da je uređaj primio smernice za saradnju tako što će pregledati **CoManagementHandler.log** na uređaju.</span><span class="sxs-lookup"><span data-stu-id="d0889-110">If the value is **Disabled** and the device is enrolled in Intune, please ensure that the device has received the Co-management policy by reviewing the **CoManagementHandler.log** on the device.</span></span>
