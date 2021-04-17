---
title: BlockLegacyAuth
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
- "3154"
- "9001194"
ms.openlocfilehash: 06ded694893c020f862864215700853b19d35f08
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820192"
---
# <a name="blocking-legacy-authentication"></a><span data-ttu-id="935ac-102">Blokiranje zatamnjene potvrde identiteta</span><span class="sxs-lookup"><span data-stu-id="935ac-102">Blocking legacy authentication</span></span>

<span data-ttu-id="935ac-103">Zatamnjena potvrda identiteta je termin koji se odnosi na zahtev za potvrdu identiteta koji je dao:</span><span class="sxs-lookup"><span data-stu-id="935ac-103">Legacy authentication is a term that refers to an authentication request made by:</span></span>

- <span data-ttu-id="935ac-104">Stariji Office klijenti koji ne koriste modernu potvrdu identiteta (na primer, Office 2010 klijent).</span><span class="sxs-lookup"><span data-stu-id="935ac-104">Older Office clients that do not use modern authentication (for example, Office 2010 client).</span></span>

- <span data-ttu-id="935ac-105">Svaki klijent koji koristi zasebne protokole pošte kao što su IMAP/SMTP/POP3.</span><span class="sxs-lookup"><span data-stu-id="935ac-105">Any client that uses legacy mail protocols such as IMAP/SMTP/POP3.</span></span>

<span data-ttu-id="935ac-106">Dodatne informacije o blokiranju zatamnjene potvrde identiteta i omogućavanju moderne potvrde identiteta potražite u temi Blokiranje [zatamnjene potvrde identiteta.](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication)</span><span class="sxs-lookup"><span data-stu-id="935ac-106">For more information on blocking legacy authentication and enabling modern authentication, refer to [Blocking legacy authentication](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-block-legacy-authentication).</span></span>

<span data-ttu-id="935ac-107">Bezbednosne podrazumevane vrednosti u Azure Active Directory (Azure AD) olakšavaju zaštitu i zaštitu vaše organizacije.</span><span class="sxs-lookup"><span data-stu-id="935ac-107">Security defaults in Azure Active Directory (Azure AD) make it easier to be secure and help protect your organization.</span></span> <span data-ttu-id="935ac-108">Podrazumevane vrednosti bezbednosti sadrže unapred konfigurisane bezbednosne postavke za uobičajene napade.</span><span class="sxs-lookup"><span data-stu-id="935ac-108">Security defaults contain preconfigured security settings for common attacks.</span></span>
<span data-ttu-id="935ac-109">Dodatne informacije o podrazumevanim vrednostima bezbednosti potražite u [temi Šta su bezbednosne podrazumevane vrednosti?.](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)</span><span class="sxs-lookup"><span data-stu-id="935ac-109">For more information about security defaults, refer to [What are security defaults?](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span></span> 

<span data-ttu-id="935ac-110">Napomi: Ako je zakupca kreiran 22. oktobra 2019. ili posle njega, moguće je da nailazite na novo bezbedno podrazumevano ponašanje i već imate omogućene podrazumevane **bezbednosne podrazumevane** vrednosti u zakupca.</span><span class="sxs-lookup"><span data-stu-id="935ac-110">**Note**:  If your tenant was created on or after October 22nd, 2019, it's possible you are experiencing the new secure-by-default behavior and already have security defaults enabled in your tenant.</span></span>  <span data-ttu-id="935ac-111">U cilju zaštite svih korisnika, bezbednosne podrazumevane vrednosti se nalaže svim novim zakucama koje su kreirali.</span><span class="sxs-lookup"><span data-stu-id="935ac-111">In an effort to protect all of our users, security defaults is being rolled out to all new tenants created.</span></span>
