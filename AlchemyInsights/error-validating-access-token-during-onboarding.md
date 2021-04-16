---
title: Došlo je do greške prilikom provere valjanosti tokena za pristup tokom nalaženja anatike radne površine
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
- "2536"
- "9000657"
ms.openlocfilehash: 12e5906ba8cbc76ba1fd99dde1cf76396c3a6942
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813702"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a><span data-ttu-id="6a1e2-102">Greška "Došlo je do greške prilikom provere valjanosti tokena za pristup" u toku ankete na radnoj površini</span><span class="sxs-lookup"><span data-stu-id="6a1e2-102">"There was an error validating access token" error during Desktop Analytics onboarding</span></span>

<span data-ttu-id="6a1e2-103">Ova greška se obično posmatra kada token potvrde identiteta istekne.</span><span class="sxs-lookup"><span data-stu-id="6a1e2-103">This error is normally observed when the authentication token expires.</span></span> <span data-ttu-id="6a1e2-104">Osvežavanje stranice obično osvežava token.</span><span class="sxs-lookup"><span data-stu-id="6a1e2-104">Usually, refreshing the page refreshes the token.</span></span> <span data-ttu-id="6a1e2-105">Međutim, ovaj problem može da potraje ako postoje neke smernice uslovnog pristupa primenjene na nalog koji se koristi za analitiku radne površine.</span><span class="sxs-lookup"><span data-stu-id="6a1e2-105">However, this issue can persist if there are any Conditional Access policies applied to the account being used to on-board Desktop Analytics.</span></span> <span data-ttu-id="6a1e2-106">Možete da pregledate Azure AD evidencije prijavljivanja na Azure portalu da biste videli da li ima neuspešnih prijavljivanja za nalog koji se koristi za ulaženje u analitiku radne površine.</span><span class="sxs-lookup"><span data-stu-id="6a1e2-106">You can review the Azure AD Sign In logs in the Azure Portal to see if there are any sign-in failures for the account being used for Desktop Analytics onboarding.</span></span>

<span data-ttu-id="6a1e2-107">Dodatne informacije o uslovnom pristupu potražite u [temi Planiranje primene uslovnog pristupa.](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access)</span><span class="sxs-lookup"><span data-stu-id="6a1e2-107">For more information about Conditional Access, visit [Plan your Conditional Access deployment](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).</span></span>