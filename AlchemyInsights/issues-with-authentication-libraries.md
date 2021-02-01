---
title: Problemi sa bibliotekama za potvrdu identiteta
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004333"
- "7731"
ms.openlocfilehash: ab4ffbc78a7cadd8acee3c98eaa5f3323da9c7e3
ms.sourcegitcommit: 7e6d89f47eca1babf5aeba4995bceccd990c3963
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 01/28/2021
ms.locfileid: "50063643"
---
# <a name="issues-with-authentication-libraries"></a><span data-ttu-id="7b089-102">Problemi sa bibliotekama za potvrdu identiteta</span><span class="sxs-lookup"><span data-stu-id="7b089-102">Issues with Authentication Libraries</span></span>

1. <span data-ttu-id="7b089-103">[Biblioteke Microsoft aplikacije za proveru](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) identiteta za identifikaciju navode na klijentske i kompatacije klijenta za Microsoft aplikacije.</span><span class="sxs-lookup"><span data-stu-id="7b089-103">[Microsoft identity platform authentication libraries](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) lists Microsoft-supported and compatible client and middleware libraries.</span></span>
2. <span data-ttu-id="7b089-104">Microsoft biblioteka autentifikacije (MSAL) podržava nekoliko [tokova autentičnosti](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows) za korišćenje u razlicitim scenarijima aplikacije.</span><span class="sxs-lookup"><span data-stu-id="7b089-104">The Microsoft Authentication Library (MSAL) supports several [authentication flows](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows) for use in different application scenarios.</span></span>
3. <span data-ttu-id="7b089-105">Da biste potvrdili identitet i nabavili Tokene, inicijalno ste pokrenuli novu javnu ili poverljivu aplikaciju klijenta u kodu.</span><span class="sxs-lookup"><span data-stu-id="7b089-105">To authenticate and acquire tokens, you initialize a new public or confidential client application in your code.</span></span> <span data-ttu-id="7b089-106">Možete da konfigurišete nekoliko opcija za konfigurisanje kada pokrenete aplikaciju klijenta u Microsoft biblioteci autentifikacije (MSAL).</span><span class="sxs-lookup"><span data-stu-id="7b089-106">You can set several configuration options when you initialize the client app in the Microsoft Authentication Library (MSAL).</span></span> <span data-ttu-id="7b089-107">Da biste saznali više, pogledajte odeljak [opcije konfiguracije aplikacija](https://docs.microsoft.com/azure/active-directory/develop/msal-client-application-configuration).</span><span class="sxs-lookup"><span data-stu-id="7b089-107">To learn more, see [Application configuration options](https://docs.microsoft.com/azure/active-directory/develop/msal-client-application-configuration).</span></span>

<span data-ttu-id="7b089-108">**Kraj podrške za Azure Active Directory potvrda identiteta biblioteke (ADALE) i Azure AD Graph Graf (AAD Graph)**</span><span class="sxs-lookup"><span data-stu-id="7b089-108">**End of support for Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph)**</span></span>

<span data-ttu-id="7b089-109">**Počevši od 30 juna, 2020**, više nećemo dodavati nove funkcije na adale i AZURE AD Graf.</span><span class="sxs-lookup"><span data-stu-id="7b089-109">**Starting June 30th, 2020**, we will no longer add any new features to ADAL and Azure AD Graph.</span></span> <span data-ttu-id="7b089-110">Nastavićemo da pružamo tehničku podršku i bezbednosne ispravke, ali više nećemo pružati ispravke funkcija.</span><span class="sxs-lookup"><span data-stu-id="7b089-110">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>

<span data-ttu-id="7b089-111">**Počevši od 30 juna, 2022**, završićemo podršku za Adale i AZURE AD Graf i neće više pružiti tehničku podršku ili bezbednosne ispravke.</span><span class="sxs-lookup"><span data-stu-id="7b089-111">**Starting June 30th, 2022**, we will end support for ADAL and Azure AD Graph and will no longer provide technical support or security updates.</span></span>

<span data-ttu-id="7b089-112">Aplikacije koje koriste ADAL na postojećim verzijama OS nastaviće da funkcionišu posle ovog vremena, ali neće *dobiti tehničku podršku ili bezbednosne ispravke*.</span><span class="sxs-lookup"><span data-stu-id="7b089-112">Apps using ADAL on existing OS versions will continue to work after this time but will not *get any technical support or security updates*.</span></span>

<span data-ttu-id="7b089-113">Aplikacije koje koriste Azure AD Graph posle ovog vremena možda više neće primati odgovore od krajnje tačke Azure oglasa Graph.</span><span class="sxs-lookup"><span data-stu-id="7b089-113">Apps using Azure AD Graph after this time may no longer receive responses from the Azure AD Graph endpoint.</span></span>

<span data-ttu-id="7b089-114">**ADALA migracija**</span><span class="sxs-lookup"><span data-stu-id="7b089-114">**ADAL Migration**</span></span>

<span data-ttu-id="7b089-115">Preporučujemo ažuriranje na [Microsoft Authentication Library (MSAL) ](https://docs.microsoft.com/azure/active-directory/develop/v2-overview)koja ima najnovije funkcije i bezbednosne ispravke.</span><span class="sxs-lookup"><span data-stu-id="7b089-115">We recommend updating to the [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), which has the latest features and security updates.</span></span>

<span data-ttu-id="7b089-116">Ako koristite Microsoft aplikacije, znajte da je Microsoft u procesu migriranja svojih aplikacija u MSAL pomoću krajnjeg roka za podršku, kako bi obezbedio korist od trenutne bezbednosti MSALA i poboljšanja funkcija.</span><span class="sxs-lookup"><span data-stu-id="7b089-116">If you are using Microsoft apps, know that Microsoft is in the process of migrating its applications to MSAL by the end-of-support deadline, ensuring they will benefit from MSAL's ongoing security and feature improvements.</span></span>

<span data-ttu-id="7b089-117">Za više informacija pogledajte članak:</span><span class="sxs-lookup"><span data-stu-id="7b089-117">For more information, see:</span></span>

1. [<span data-ttu-id="7b089-118">Pročitajte najčešća pitanja za ADAL</span><span class="sxs-lookup"><span data-stu-id="7b089-118">Read the ADAL FAQ</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [<span data-ttu-id="7b089-119">Saznajte više o tome kako da migrirate aplikacije na osnovu platforme</span><span class="sxs-lookup"><span data-stu-id="7b089-119">Learn about how to migrate apps on a per-platform basis</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. <span data-ttu-id="7b089-120">Ako vam je potrebna pomoć da biste razumeli koje aplikacije koriste ADALE, preporučujemo da pregledate sve izvorne kodove za aplikacije i ako je to primenljivo, da pristupite bilo kom dobavljaču ili dobavljačima aplikacija.</span><span class="sxs-lookup"><span data-stu-id="7b089-120">If you need help understanding which of your apps use ADAL, we recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="7b089-121">Microsoft podrška vam takođe može pružiti listu svih aplikacija koje nisu Microsoft ADAL u vašem zakupcu.</span><span class="sxs-lookup"><span data-stu-id="7b089-121">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>

<span data-ttu-id="7b089-122">**AAD Graph migracija**</span><span class="sxs-lookup"><span data-stu-id="7b089-122">**AAD Graph Migration**</span></span>

<span data-ttu-id="7b089-123">Za aplikacije koje koriste Azure AD Graph, potražite uputstvo za [migraciju AZURE AD Graph grafika u Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview).</span><span class="sxs-lookup"><span data-stu-id="7b089-123">For applications that are using Azure AD Graph, follow our guidance to [migrate Azure AD Graph apps to Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview).</span></span>

1. [<span data-ttu-id="7b089-124">Naša kontrolna lista za migraciju pruža taиku na početku.</span><span class="sxs-lookup"><span data-stu-id="7b089-124">Our migration checklist provides a getting started point.</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)
2. <span data-ttu-id="7b089-125">Vaš portal za registraciju aplikacija Azure prikazuje koje aplikacije koriste AAD Graph.</span><span class="sxs-lookup"><span data-stu-id="7b089-125">Your Azure app registration portal shows which applications are using AAD Graph.</span></span> <span data-ttu-id="7b089-126">Preporučujemo vam da pregledate sav izvorni kod aplikacija i, ako je primenljivo, kontaktirate bilo koje ISV-ove ili dobavljače aplikacija.</span><span class="sxs-lookup"><span data-stu-id="7b089-126">We recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="7b089-127">Microsoft podrška vam takođe može pružiti listu svih podrške za AAD Graph u zakupcu.</span><span class="sxs-lookup"><span data-stu-id="7b089-127">Microsoft support can also provide you with a list of all AAD Graph usage in your tenant.</span></span>
3. <span data-ttu-id="7b089-128">Da bi aplikacija pristupala podacima u programu Microsoft Graph, korisnik ili administrator mora da joj dodeli ispravne dozvole putem procesa pristanka.</span><span class="sxs-lookup"><span data-stu-id="7b089-128">For your app to access data in Microsoft Graph, the user or administrator must grant it the correct permissions via a consent process.</span></span> <span data-ttu-id="7b089-129">[Referenca sa Microsoft Graph dozvolama](https://docs.microsoft.com/graph/permissions-reference) navodi dozvole povezane sa svakim glavnim skupom Microsoft Graph API.</span><span class="sxs-lookup"><span data-stu-id="7b089-129">The [Microsoft Graph permissions reference](https://docs.microsoft.com/graph/permissions-reference) lists the permissions associated with each major set of Microsoft Graph APIs.</span></span> <span data-ttu-id="7b089-130">On takođe pruža uputstva o tome kako da koristite dozvole.</span><span class="sxs-lookup"><span data-stu-id="7b089-130">It also provides guidance about how to use the permissions.</span></span>
