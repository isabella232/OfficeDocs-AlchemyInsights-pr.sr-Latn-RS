---
title: Rešavanje problema sa sinhronizacijom lozinki
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: 96f63f2ae8e5de246bce7fc15a9b2c3d604f2eb8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664940"
---
# <a name="troubleshoot-password-synchronization"></a><span data-ttu-id="6f06f-102">Rešavanje problema sa sinhronizacijom lozinki</span><span class="sxs-lookup"><span data-stu-id="6f06f-102">Troubleshoot password synchronization</span></span>

<span data-ttu-id="6f06f-103">Da biste rešili probleme sa sinhronizacijom lozinki, počnite pomoću ovog zadatka za rešavanje problema sa AAD povezivanjem da biste utvrdili zašto se lozinke ne sinhronizuju.</span><span class="sxs-lookup"><span data-stu-id="6f06f-103">To troubleshoot password synchronization issues, start by using this AAD Connect troubleshooting task to determine why passwords are not syncing.</span></span> <span data-ttu-id="6f06f-104">Da biste počeli, idite na [Upravljanje direktnom sinhronizacijom](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).</span><span class="sxs-lookup"><span data-stu-id="6f06f-104">To begin, go to [Manage direct sync](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).</span></span>  

1. <span data-ttu-id="6f06f-105">Otvorite novu sesiju Windows PowerShell na Azure AD Connect serveru i izaberite opciju " **pokrene kao administrator** ".</span><span class="sxs-lookup"><span data-stu-id="6f06f-105">Open a new Windows PowerShell session on your Azure AD Connect server, and select the **Run as Administrator** option.</span></span>

2. <span data-ttu-id="6f06f-106">Neograničeno je potpisano ili izvršeno izvršeno smernice za stavku radi izvršenih smernica.</span><span class="sxs-lookup"><span data-stu-id="6f06f-106">Run Set-ExecutionPolicy RemoteSigned or Set-ExecutionPolicy Unrestricted.</span></span>

3. <span data-ttu-id="6f06f-107">Pokrenite čarobnjak za Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="6f06f-107">Start the Azure AD Connect wizard.</span></span>

4. <span data-ttu-id="6f06f-108">Idite na stranicu dodatne zadatke > **rešite problem**  >  **dalje**.</span><span class="sxs-lookup"><span data-stu-id="6f06f-108">Go to the Additional Tasks page > **Troubleshoot** > **Next**.</span></span>

5. <span data-ttu-id="6f06f-109">Izaberite stavku **pokretanje** da biste otvorili meni za rešavanje problema sa PowerShell.</span><span class="sxs-lookup"><span data-stu-id="6f06f-109">Select **Launch** to open the PowerShell troubleshooting menu.</span></span>

6. <span data-ttu-id="6f06f-110">Izaberite stavku **Rešavanje problema sa sinhronizacijom lozinki**.</span><span class="sxs-lookup"><span data-stu-id="6f06f-110">Select **Troubleshoot Password Synchronization**.</span></span>

    <span data-ttu-id="6f06f-111">Problem je obično da se lozinka ne sinhronizuje za određeni korisnički nalog.</span><span class="sxs-lookup"><span data-stu-id="6f06f-111">The issue is usually that a password is not synchronized for a specific user account.</span></span>

    <span data-ttu-id="6f06f-112">**Beleške** Sinhronizacija lozinki ne uspeva ako je prethodna sinhronizacija lozinki nedavno proљla.</span><span class="sxs-lookup"><span data-stu-id="6f06f-112">**Notes** Password synchronization fails if the last successful password sync was some time ago.</span></span>

<span data-ttu-id="6f06f-113">Dodatne pomoći za rešavanje problema sa sinhronizacijom lozinki potražite [u članku rešavanje problema sa hash sinhronizacijom lozinki pomoću usluge Azure AD Connect Sync](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span><span class="sxs-lookup"><span data-stu-id="6f06f-113">For more help troubleshooting password synchronization, see [Troubleshoot password hash synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span></span>