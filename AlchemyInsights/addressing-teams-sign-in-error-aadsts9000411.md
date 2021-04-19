---
title: Addressing Teams greška pri prijavljivanjem AADSTS9000411
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
- "9000744"
- "5689"
ms.openlocfilehash: 7b0e90e3fea716df649ec906ad8b3008386684be
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/15/2021
ms.locfileid: "51822001"
---
# <a name="addressing-teams-sign-in-error-aadsts9000411"></a><span data-ttu-id="f308c-102">Addressing Teams greška pri prijavljivanjem AADSTS9000411</span><span class="sxs-lookup"><span data-stu-id="f308c-102">Addressing Teams sign-in error AADSTS9000411</span></span>

<span data-ttu-id="f308c-103">Prilikom prijave u Microsoft Teams, možda ćete dobiti grešku: Žao nam je, ali imamo problema sa prijavljivanjem u **AADSTS9000411: Zahtev nije ispravno oblikovan. Parametar "login_hint" se duplira.**</span><span class="sxs-lookup"><span data-stu-id="f308c-103">When signing in to Microsoft Teams, you may receive the error: **Sorry, but we're having trouble with signing you in AADSTS9000411: The request is not properly formatted. The parameter "login_hint" is duplicated.**</span></span>

<span data-ttu-id="f308c-104">Da biste rešili ovaj problem, uverite se da su Microsoft Teams klijenti ažurirani.</span><span class="sxs-lookup"><span data-stu-id="f308c-104">To address this issue, please ensure your Microsoft Teams clients are updated.</span></span> <span data-ttu-id="f308c-105">Dodatne informacije o ažuriranju klijenta potražite u članku [Ažuriranje usluge Microsoft Teams.](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1)</span><span class="sxs-lookup"><span data-stu-id="f308c-105">For more information on updating your client, see [Update Microsoft Teams](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

<span data-ttu-id="f308c-106">Ako iz nekog razloga ne možete da ažurirate klijenta, odjavljanje klijenta će obrtati većinu kešnih podataka.</span><span class="sxs-lookup"><span data-stu-id="f308c-106">If you cannot update your client for some reason, logging off the client will clear most cached data.</span></span> <span data-ttu-id="f308c-107">Međutim, ako i dalje imate problema posle prijavljivanja/prijavljivanja, zatvorite Teams i obrišite keš klijenta tako što ćete uraditi sledeće:</span><span class="sxs-lookup"><span data-stu-id="f308c-107">However, if you still have issues after logoff/logon, quit Teams and please clear your client cache by doing the following:</span></span>
1. <span data-ttu-id="f308c-108">Zatvorite Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="f308c-108">Close Microsoft Teams.</span></span>
2. <span data-ttu-id="f308c-109">Idite na: %appdata%\microsoft\teams i izbrišite sve datoteke.</span><span class="sxs-lookup"><span data-stu-id="f308c-109">Go to: %appdata%\microsoft\teams and delete all the files.</span></span>
3. <span data-ttu-id="f308c-110">Ponovo otvorite Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="f308c-110">Reopen Microsoft Teams.</span></span>
