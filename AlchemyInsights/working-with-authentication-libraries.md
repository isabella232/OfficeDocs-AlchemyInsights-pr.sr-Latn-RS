---
title: Rad sa bibliotekama za potvrdu identiteta
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9775"
- "9004342"
ms.openlocfilehash: f9f54ed2bfc5841df66d3e714112b9307455c182
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036870"
---
# <a name="working-with-authentication-libraries"></a><span data-ttu-id="a2ab3-102">Rad sa bibliotekama za potvrdu identiteta</span><span class="sxs-lookup"><span data-stu-id="a2ab3-102">Working with Authentication Libraries</span></span>

<span data-ttu-id="a2ab3-103">Da biste rešili problem sa Microsoft bibliotekom identiteta (MSAL), obavite sledeće preporučene korake:</span><span class="sxs-lookup"><span data-stu-id="a2ab3-103">To resolve Microsoft Authentication Library (MSAL) issue, perform the following recommended steps:</span></span>

1. <span data-ttu-id="a2ab3-104">**Rad sa uslugom MSAL**: [bibliotekama za potvrdu identiteta Microsoft platforme](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) – ovaj članak prikazuje podršku za Microsoft biblioteku za Microsoft potvrdu identiteta za nekoliko tipova aplikacija.</span><span class="sxs-lookup"><span data-stu-id="a2ab3-104">**Working with MSAL**: [Microsoft identity platform authentication libraries](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) - This article shows Microsoft Authentication Library support for several application types.</span></span> <span data-ttu-id="a2ab3-105">On uključuje veze ka izvornom kodu biblioteke; Gde da nabavite paket za projekat aplikacije? i da li biblioteka podržava korisničko prijavljivanje (potvrda identiteta), pristup zaštićenom vebu Appis (autorizaciju) ili oba.</span><span class="sxs-lookup"><span data-stu-id="a2ab3-105">It includes links to library source code; where to get the package for your app's project; and whether the library supports user sign-in (authentication), access to protected web APIs (authorization), or both.</span></span>

2. <span data-ttu-id="a2ab3-106">**Rešavanje problema sa autentifikacijom**: msal podržava nekoliko tokova autentičnosti za korišćenje u razlicitim scenarijima aplikacije.</span><span class="sxs-lookup"><span data-stu-id="a2ab3-106">**Troubleshoot Authentication**: The MSAL supports several authentication flows for use in different application scenarios.</span></span> <span data-ttu-id="a2ab3-107">U zavisnosti od toga kako se gradi klijentska aplikacija, MSAL može da koristi neki od tokova potvrde identiteta koje podržava Microsoft Platform identiteta.</span><span class="sxs-lookup"><span data-stu-id="a2ab3-107">Depending on how your client application is built, the MSAL can use one or more of the authentication flows supported by the Microsoft identity platform.</span></span> <span data-ttu-id="a2ab3-108">Ovi tokovi mogu da proizvedu nekoliko tipova pozivnih brojeva i kodova za autorizaciju i zahtevaju razne simbole da bi radili.</span><span class="sxs-lookup"><span data-stu-id="a2ab3-108">These flows can produce several types of tokens and authorization codes, and require different tokens to make them work.</span></span>

3. <span data-ttu-id="a2ab3-109">**Access tokena**: [microsoftens Platform za identifikaciju identiteta](https://docs.microsoft.com/azure/active-directory/develop/access-tokens) – Saznajte kako API može da proveri valjanost i koristi zahteve unutar simbola za pristup.</span><span class="sxs-lookup"><span data-stu-id="a2ab3-109">**Access Tokens**: [Microsoft identity platform access tokens](https://docs.microsoft.com/azure/active-directory/develop/access-tokens) - Learn how your API can validate and use the claims inside an access token.</span></span> <span data-ttu-id="a2ab3-110">Sva dokumentacija u ovom članku, osim gde je navedeno, odnosi se samo na Tokene koji su izdati za APIs koje ste registrovali.</span><span class="sxs-lookup"><span data-stu-id="a2ab3-110">All documentation in this article, except where noted, applies only to tokens issued for APIs you've registered.</span></span> <span data-ttu-id="a2ab3-111">Ne odnosi se na oznake koje su izdate za usluge koje posjeduje Microsoft-not, niti se ovi Tokeni mogu koristiti za validaciju načina na koji Microsoft platforma za identifikaciju izdaje tokena za API koji kreirate.</span><span class="sxs-lookup"><span data-stu-id="a2ab3-111">It does not apply to tokens issued for Microsoft-owned APIs, nor can those tokens be used to validate how the Microsoft identity platform will issue tokens for an API you create.</span></span>

<span data-ttu-id="a2ab3-112">**Kraj podrške za Azure Active Directory potvrda verodostojnosti (ADALE)**</span><span class="sxs-lookup"><span data-stu-id="a2ab3-112">**End of support for Azure Active Directory Authentication Library (ADAL)**</span></span>

- <span data-ttu-id="a2ab3-113">**Počevši od 30 juna, 2020,** više nećemo dodavati nove funkcije na adale i AZURE AD Graf.</span><span class="sxs-lookup"><span data-stu-id="a2ab3-113">**Starting June 30th, 2020,** we will no longer add any new features to ADAL and Azure AD Graph.</span></span> <span data-ttu-id="a2ab3-114">Nastavićemo da pružamo tehničku podršku i bezbednosne ispravke, ali više nećemo pružati ispravke funkcija.</span><span class="sxs-lookup"><span data-stu-id="a2ab3-114">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>
- <span data-ttu-id="a2ab3-115">**Počevši od 30 juna, 2022,** Završićemo podršku za Adale i AZURE AD Graf i neće više pružiti tehničku podršku ili bezbednosne ispravke.</span><span class="sxs-lookup"><span data-stu-id="a2ab3-115">**Starting June 30th, 2022,** we will end support for ADAL and Azure AD Graph and will no longer provide technical support or security updates.</span></span>
- <span data-ttu-id="a2ab3-116">Aplikacije koje koriste ADAL na postojećim verzijama OS nastaviće da funkcionišu posle ovog vremena, ali neće *dobiti tehničku podršku ili bezbednosne ispravke*.</span><span class="sxs-lookup"><span data-stu-id="a2ab3-116">Apps using ADAL on existing OS versions will continue to work after this time but will not *get any technical support or security updates*.</span></span>
- <span data-ttu-id="a2ab3-117">Aplikacije koje koriste Azure AD Graph posle ovog vremena možda više neće primati odgovore od krajnje tačke Azure oglasa Graph.</span><span class="sxs-lookup"><span data-stu-id="a2ab3-117">Apps using Azure AD Graph after this time may no longer receive responses from the Azure AD Graph endpoint.</span></span>

<span data-ttu-id="a2ab3-118">**ADALA migracija**</span><span class="sxs-lookup"><span data-stu-id="a2ab3-118">**ADAL Migration**</span></span>

- <span data-ttu-id="a2ab3-119">Preporučujemo da ažurirate MSAL, koji ima najnovije funkcije i bezbednosne ispravke.</span><span class="sxs-lookup"><span data-stu-id="a2ab3-119">We recommend updating to the MSAL, which has the latest features and security updates.</span></span>
- <span data-ttu-id="a2ab3-120">Ako koristite Microsoft aplikacije, znajte da je Microsoft u procesu migriranja svojih aplikacija u MSAL pomoću krajnjeg roka za podršku, kada se osigura da će imati koristi od MSALOVE trenutne bezbednosti i poboljšanja funkcija.</span><span class="sxs-lookup"><span data-stu-id="a2ab3-120">If you're using Microsoft apps, know that Microsoft is in the process of migrating its apps to MSAL by the end-of-support deadline, ensuring they'll benefit from MSAL's ongoing security and feature improvements.</span></span>

1. <span data-ttu-id="a2ab3-121">[Pročitajte Adala najčešća pitanja](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span><span class="sxs-lookup"><span data-stu-id="a2ab3-121">[Read the ADAL FAQ](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span></span>
2. <span data-ttu-id="a2ab3-122">[Saznajte kako da migrirate aplikacije na osnovu osnove po platformoji](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#migration-guidance).</span><span class="sxs-lookup"><span data-stu-id="a2ab3-122">[Learn about how to migrate apps on a per-platform basis](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#migration-guidance).</span></span>
3. <span data-ttu-id="a2ab3-123">Ako nakon čitanja vodiča za platformu aplikacije imate dodatna pitanja, možete da knjižite na [lokaciji Microsoft Q&](https://docs.microsoft.com/answers/topics/azure-ad-adal-deprecation.html) sa oznakom [azuri-AD-dprecation] ili da otvorite problem u programu GitHub biblioteke.</span><span class="sxs-lookup"><span data-stu-id="a2ab3-123">If, after reading the guide for your app's platform, you have additional questions, you can post on [Microsoft Q&A](https://docs.microsoft.com/answers/topics/azure-ad-adal-deprecation.html) with the tag [azure-ad-adal-deprecation] or open an issue in library's GitHub repository.</span></span> <span data-ttu-id="a2ab3-124">Pogledajte odeljak [jezici i okviri](https://docs.microsoft.com/azure/active-directory/develop/msal-overview#languages-and-frameworks) **prikaza teksta za veze sa** potvrdom svake biblioteke.</span><span class="sxs-lookup"><span data-stu-id="a2ab3-124">See the [Languages and frameworks](https://docs.microsoft.com/azure/active-directory/develop/msal-overview#languages-and-frameworks) section of the **MSAL overview** article for links to each library's repo.</span></span>
4. <span data-ttu-id="a2ab3-125">**Ako vam je potrebna pomoć da biste razumeli koje aplikacije koriste adno**, preporučujemo vam da pregledate sve izvorne kodove za aplikacije.</span><span class="sxs-lookup"><span data-stu-id="a2ab3-125">**If you need help understanding which of your apps use ADAL**, we recommend you review all of your apps' source code.</span></span> <span data-ttu-id="a2ab3-126">Ako je to primenljivo, pristupite bilo kom nezavisnom dobavljaču usluga (ISVs) ili dobavljačima aplikacija.</span><span class="sxs-lookup"><span data-stu-id="a2ab3-126">If applicable, reach out to any Independent software vendors (ISVs) or app providers.</span></span> <span data-ttu-id="a2ab3-127">Microsoft podrška vam takođe može pružiti listu svih aplikacija koje nisu Microsoft ADAL u vašem zakupcu.</span><span class="sxs-lookup"><span data-stu-id="a2ab3-127">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>







