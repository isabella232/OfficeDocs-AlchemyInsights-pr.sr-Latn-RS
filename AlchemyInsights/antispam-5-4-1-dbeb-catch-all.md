---
title: AntiSpam 5.4.1 DBEB
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001209"
- "3167"
ms.openlocfilehash: f9d613457ae33dc7e00f20391bbdff029500a123
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47717375"
---
# <a name="fix-delivery-issues-for-error-code-550-541-relay-access-denied"></a><span data-ttu-id="57a7d-102">Rešavanje problema sa isporukom za kôd greške 550 5.4.1 pristup relej zabranjen</span><span class="sxs-lookup"><span data-stu-id="57a7d-102">Fix delivery issues for error code 550 5.4.1 Relay Access Denied</span></span>

<span data-ttu-id="57a7d-103">Do ovog problema dolazi prilikom [provere da biste videli da li je adresa e-pošte važeća da biste sprečili](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) pretplatu prilikom ulaska u Microsoft Network.</span><span class="sxs-lookup"><span data-stu-id="57a7d-103">This problem occurs when [checking to see if an email address is valid to prevent bouncebacks](https://docs.microsoft.com/exchange/mail-flow-best-practices/use-directory-based-edge-blocking) when entering the Microsoft network.</span></span> <span data-ttu-id="57a7d-104">Isprobajte sledeće:</span><span class="sxs-lookup"><span data-stu-id="57a7d-104">Try the following:</span></span>

1. <span data-ttu-id="57a7d-105">Utvrdite da li je problem karakterističan za ceo domen ili jednu e-adresu:</span><span class="sxs-lookup"><span data-stu-id="57a7d-105">Determine whether the problem is specific to an entire domain or a single email address:</span></span>
    - <span data-ttu-id="57a7d-106">Ceo domen: ponekad domen treba da se sinhronizuje; Pokušajte da [postavite domen na unutrašnju, a zatim na autoritativno](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span><span class="sxs-lookup"><span data-stu-id="57a7d-106">Entire domain: Sometimes the domain needs to be synchronized; try [setting the domain to Internal and then back to Authoritative](https://docs.microsoft.com/exchange/mail-flow-best-practices/manage-accepted-domains/manage-accepted-domains).</span></span>
    - <span data-ttu-id="57a7d-107">Jedinstvena e-adresa: ponekad treba da se sinhronizuje adresa; Promena SMTP proxy adrese, a zatim promena može da pomogne.</span><span class="sxs-lookup"><span data-stu-id="57a7d-107">Single email address: Sometimes the address needs to be synchronized; changing the smtp proxy address and then changing it back can help.</span></span>
2. <span data-ttu-id="57a7d-108">Utvrdite da li je problem karakterističan za grupu ili javnu fasciklu.</span><span class="sxs-lookup"><span data-stu-id="57a7d-108">Determine whether the problem is specific to a group or public folder.</span></span> <span data-ttu-id="57a7d-109">Za neke tipove objekata možda će biti potrebno da se objekti ručno kreiraju u usluzi Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="57a7d-109">For some object types, the objects may need to be manually created in Azure Active Directory.</span></span>

<span data-ttu-id="57a7d-110">Ako vam je potrebna dodatna pomoć, otvorite ulaznicu za podršku i navedite opseg problema (uključujući tip objekta u koji šaljete) kako bismo vam lakše pomogli.</span><span class="sxs-lookup"><span data-stu-id="57a7d-110">If you need additional help, please open a support ticket and specify the scope of the issue (including the type of object you're sending to) so we can assist you better.</span></span>