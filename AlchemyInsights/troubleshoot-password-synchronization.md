---
title: Rešavanje problema sa sinhronizacijom lozinke
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: 54b5a033b7cbb99520425b31800364ed4a99a4e6
ms.sourcegitcommit: 1d01b8b48eef2d5d10c375dcf802cd36e9d6bf61
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 07/23/2020
ms.locfileid: "45387891"
---
# <a name="troubleshoot-password-synchronization"></a><span data-ttu-id="6156d-102">Rešavanje problema sa sinhronizacijom lozinke</span><span class="sxs-lookup"><span data-stu-id="6156d-102">Troubleshoot password synchronization</span></span>

<span data-ttu-id="6156d-103">Da biste rešili probleme sa sinhronizacijom lozinke, počnite tako što ćete koristiti ovaj zadatak rešavanja problema u vezi sa povezivanjem da biste utvrdili zašto se lozinke ne sinhronizuju.</span><span class="sxs-lookup"><span data-stu-id="6156d-103">To troubleshoot password synchronization issues, start by using this AAD Connect troubleshooting task to determine why passwords are not syncing.</span></span> <span data-ttu-id="6156d-104">Da biste počeli, idite na [Upravljanje direktnom sinhronizacijom](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).</span><span class="sxs-lookup"><span data-stu-id="6156d-104">To begin, go to [Manage direct sync](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).</span></span>  

1. <span data-ttu-id="6156d-105">Otvorite novu sesiju Windows PowerShell na serveru za povezivanje sa Azure serverom, a zatim izaberite opciju " **Pokreni kao administrator** ".</span><span class="sxs-lookup"><span data-stu-id="6156d-105">Open a new Windows PowerShell session on your Azure AD Connect server, and select the **Run as Administrator** option.</span></span>

2. <span data-ttu-id="6156d-106">Pokretanje set-izvršne smernice RemoteSigned ili set-izvršne smernice neograničeno.</span><span class="sxs-lookup"><span data-stu-id="6156d-106">Run Set-ExecutionPolicy RemoteSigned or Set-ExecutionPolicy Unrestricted.</span></span>

3. <span data-ttu-id="6156d-107">Pokrenite čarobnjak za povezivanje "Azure AD".</span><span class="sxs-lookup"><span data-stu-id="6156d-107">Start the Azure AD Connect wizard.</span></span>

4. <span data-ttu-id="6156d-108">Idite na stranicu "dodatni zadaci" > **rešiti problem**  >  **dalje**.</span><span class="sxs-lookup"><span data-stu-id="6156d-108">Go to the Additional Tasks page > **Troubleshoot** > **Next**.</span></span>

5. <span data-ttu-id="6156d-109">Izaberite " **Pokreni** " da biste otvorili meni "Rešavanje problema sa PowerShell".</span><span class="sxs-lookup"><span data-stu-id="6156d-109">Select **Launch** to open the PowerShell troubleshooting menu.</span></span>

6. <span data-ttu-id="6156d-110">Izaberite **Rešavanje problema sa sinhronizacijom lozinke**.</span><span class="sxs-lookup"><span data-stu-id="6156d-110">Select **Troubleshoot Password Synchronization**.</span></span>

    <span data-ttu-id="6156d-111">Ovo pitanje obično znači da lozinka nije sinhronizovana za određeni korisnički nalog.</span><span class="sxs-lookup"><span data-stu-id="6156d-111">The issue is usually that a password is not synchronized for a specific user account.</span></span>

    <span data-ttu-id="6156d-112">**Notes** Sinhronizacija lozinke nije uspela ako je poslednja uspešna sinhronizacija lozinke bila pre izvesnog vremena.</span><span class="sxs-lookup"><span data-stu-id="6156d-112">**Notes** Password synchronization fails if the last successful password sync was some time ago.</span></span>

<span data-ttu-id="6156d-113">Da biste dobili dodatnu pomoć za rešavanje problema sa lozinkom sinhronizacija, pogledajte odeljak [Rešavanje problema sa lozinkom lozinka za sinhronizaciju pomoću programa Azure sinhr](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span><span class="sxs-lookup"><span data-stu-id="6156d-113">For more help troubleshooting password synchronization, see [Troubleshoot password hash synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span></span>