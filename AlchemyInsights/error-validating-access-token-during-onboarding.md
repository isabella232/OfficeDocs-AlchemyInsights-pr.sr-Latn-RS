---
title: Došlo je do greške prilikom ispravnosti greške Token za pristup tokom analitike radne površine na sajtu
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
- "2536"
- "9000657"
ms.openlocfilehash: 45c6fb1a1632799a07c028c0791b6b8e77635293
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/15/2020
ms.locfileid: "47783565"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a><span data-ttu-id="4fc51-102">"Došlo je do greške prilikom ispravljanja simbola za Access tokom Analizata radne površine</span><span class="sxs-lookup"><span data-stu-id="4fc51-102">"There was an error validating access token" error during Desktop Analytics onboarding</span></span>

<span data-ttu-id="4fc51-103">Ova greška se obično posmatra kada istekne simbol potvrde identiteta.</span><span class="sxs-lookup"><span data-stu-id="4fc51-103">This error is normally observed when the authentication token expires.</span></span> <span data-ttu-id="4fc51-104">Osvežavanje stranice obično osvežava simbol.</span><span class="sxs-lookup"><span data-stu-id="4fc51-104">Usually, refreshing the page refreshes the token.</span></span> <span data-ttu-id="4fc51-105">Međutim, ovaj problem može da bude istrajen ako postoji neka uslovna smernica za pristup koja se primenjuju na nalog koji se koristi za analitiku na računaru.</span><span class="sxs-lookup"><span data-stu-id="4fc51-105">However, this issue can persist if there are any Conditional Access policies applied to the account being used to on-board Desktop Analytics.</span></span> <span data-ttu-id="4fc51-106">Možete da pregledate upitnik Azure AD u evidenciji na Azure sajtu da biste videli da li postoje promaљaji za prijavljivanje za nalog koji se koristi za Online analitiku.</span><span class="sxs-lookup"><span data-stu-id="4fc51-106">You can review the Azure AD Sign In logs in the Azure Portal to see if there are any sign-in failures for the account being used for Desktop Analytics onboarding.</span></span>

<span data-ttu-id="4fc51-107">Više informacija o uslovnom pristupu potražite u članku [Planiranje uslovnog pristupa](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).</span><span class="sxs-lookup"><span data-stu-id="4fc51-107">For more information about Conditional Access, visit [Plan your Conditional Access deployment](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).</span></span>