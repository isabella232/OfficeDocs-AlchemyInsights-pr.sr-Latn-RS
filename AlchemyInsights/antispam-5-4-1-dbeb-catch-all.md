---
title: AntiSpam 5.4.1 DBEB catch-all
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001209"
- "3167"
ms.openlocfilehash: c6ce26a133428dc7351912d8250ef096dfc7521a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821461"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a><span data-ttu-id="81ca5-102">Rešavanje problema sa isporukom za kôd greške 550 5.4.1 Relay Access Denied</span><span class="sxs-lookup"><span data-stu-id="81ca5-102">Fix delivery issues for error code 550 5.4.1 Relay Access Denied</span></span>

<span data-ttu-id="81ca5-103">Do ovog problema dolazi prilikom [provere da li](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) je e-adresa važeća za sprečavanje povratnih grešaka prilikom ulaska na Microsoft mrežu.</span><span class="sxs-lookup"><span data-stu-id="81ca5-103">This problem occurs when [checking to see if an email address is valid to prevent bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) when entering the Microsoft network.</span></span> <span data-ttu-id="81ca5-104">Pokušajte sledeće:</span><span class="sxs-lookup"><span data-stu-id="81ca5-104">Try the following:</span></span>

1. <span data-ttu-id="81ca5-105">Utvrdite da li je problem specifičan za ceo domen ili za jednu e-adresu:</span><span class="sxs-lookup"><span data-stu-id="81ca5-105">Determine whether the problem is specific to an entire domain or a single email address:</span></span>
    - <span data-ttu-id="81ca5-106">Ceo domen: Domen ponekad treba da se sinhronizuje; pokušajte [da podešavanje domena na Interni, a zatim se vratite na ovlašćeni](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span><span class="sxs-lookup"><span data-stu-id="81ca5-106">Entire domain: Sometimes the domain needs to be synchronized; try [setting the domain to Internal and then back to Authoritative](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span></span>
    - <span data-ttu-id="81ca5-107">Jedna adresa e-pošte: Ponekad adresa treba da se sinhronizuje; promena smtp proxy adrese, a zatim promena nazad može pomoći.</span><span class="sxs-lookup"><span data-stu-id="81ca5-107">Single email address: Sometimes the address needs to be synchronized; changing the smtp proxy address and then changing it back can help.</span></span>
2. <span data-ttu-id="81ca5-108">Utvrdite da li je problem specifičan za grupu ili javnu fasciklu.</span><span class="sxs-lookup"><span data-stu-id="81ca5-108">Determine whether the problem is specific to a group or public folder.</span></span> <span data-ttu-id="81ca5-109">Za neke tipove objekata ćete možda morati ručno da kreirate u Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="81ca5-109">For some object types, the objects may need to be manually created in Azure Active Directory.</span></span>

<span data-ttu-id="81ca5-110">Ako vam je potrebna dodatna pomoć, otvorite tiket za podršku i navedite polje problema (uključujući tip objekta na koji šaljete) kako bismo vam pomogli bolje.</span><span class="sxs-lookup"><span data-stu-id="81ca5-110">If you need additional help, please open a support ticket and specify the scope of the issue (including the type of object you're sending to) so we can assist you better.</span></span>