---
title: Problemi sa razvojem aplikacija sa Appis
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004343"
- "7755"
ms.openlocfilehash: 26d732819b64efa4fb84da44cc2a279368aa28b0
ms.sourcegitcommit: 605a73b159d30634b064c1b63b0e734ceb3fdec8
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 01/25/2021
ms.locfileid: "49975016"
---
# <a name="issues-developing-applications-with-apis"></a><span data-ttu-id="9fac2-102">Problemi sa razvojem aplikacija sa Appis</span><span class="sxs-lookup"><span data-stu-id="9fac2-102">Issues developing applications with APIs</span></span>

<span data-ttu-id="9fac2-103">Da biste počeli da koristite Azure Active Directory Graph API, pogledajte " [AZURE AD Graph grafikon" brzi Start "vodiča](https://docs.microsoft.com/azure/active-directory/develop/microsoft-graph-intro) ili Prikažite [interaktivnu dokumentaciju Azure AD Graph AD Graph](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/api-catalog).</span><span class="sxs-lookup"><span data-stu-id="9fac2-103">To begin using the Azure Active Directory Graph API, see the [Azure AD Graph API quickstart guide](https://docs.microsoft.com/azure/active-directory/develop/microsoft-graph-intro) , or view the [interactive Azure AD Graph API reference documentation](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/api-catalog).</span></span>

<span data-ttu-id="9fac2-104">**Kraj podrške za Azure Active Directory potvrda identiteta biblioteke (ADALE) i Azure AD Graph Graf (AAD Graph)**</span><span class="sxs-lookup"><span data-stu-id="9fac2-104">**End of support for Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph)**</span></span>

<span data-ttu-id="9fac2-105">**Počevši od 30 juna, 2020**, više nećemo dodavati nove funkcije na adale i AZURE AD Graf.</span><span class="sxs-lookup"><span data-stu-id="9fac2-105">**Starting June 30th, 2020**, we will no longer add any new features to ADAL and Azure AD Graph.</span></span> <span data-ttu-id="9fac2-106">Nastavićemo da pružamo tehničku podršku i bezbednosne ispravke, ali više nećemo pružati ispravke funkcija.</span><span class="sxs-lookup"><span data-stu-id="9fac2-106">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>

<span data-ttu-id="9fac2-107">**Počevši od 30 juna, 2022**, završićemo podršku za Adale i AZURE AD Graf i neće više pružiti tehničku podršku ili bezbednosne ispravke.</span><span class="sxs-lookup"><span data-stu-id="9fac2-107">**Starting June 30th, 2022**, we will end support for ADAL and Azure AD Graph and will no longer provide technical support or security updates.</span></span>

<span data-ttu-id="9fac2-108">Aplikacije koje koriste ADAL na postojećim verzijama OS nastaviće da funkcionišu posle ovog vremena, ali neće dobiti tehničku podršku ili bezbednosne ispravke.</span><span class="sxs-lookup"><span data-stu-id="9fac2-108">Apps using ADAL on existing OS versions will continue to work after this time but will not get any technical support or security updates.</span></span>

<span data-ttu-id="9fac2-109">Aplikacije koje koriste Azure AD Graph posle ovog vremena možda više neće primati odgovore od krajnje tačke Azure oglasa Graph.</span><span class="sxs-lookup"><span data-stu-id="9fac2-109">Apps using Azure AD Graph after this time may no longer receive responses from the Azure AD Graph endpoint.</span></span>

<span data-ttu-id="9fac2-110">**ADALA migracija**</span><span class="sxs-lookup"><span data-stu-id="9fac2-110">**ADAL Migration**</span></span>

<span data-ttu-id="9fac2-111">Preporučujemo da ažurirate u [Microsoft biblioteci autentifikacije (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), koja ima najnovije funkcije i bezbednosne ispravke.</span><span class="sxs-lookup"><span data-stu-id="9fac2-111">We recommend updating to the [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), which has the latest features and security updates.</span></span>

<span data-ttu-id="9fac2-112">Ako koristite Microsoft aplikacije, znajte da je Microsoft u procesu migriranja svojih aplikacija u MSAL pomoću krajnjeg roka za podršku, kada se osigura da će imati koristi od MSALOVE trenutne bezbednosti i poboljšanja funkcija.</span><span class="sxs-lookup"><span data-stu-id="9fac2-112">If you're using Microsoft apps, know that Microsoft is in the process of migrating its applications to MSAL by the end-of-support deadline, ensuring they'll benefit from MSAL's ongoing security and feature improvements.</span></span>

1. <span data-ttu-id="9fac2-113">[Pročitajte Adala najčešća pitanja](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span><span class="sxs-lookup"><span data-stu-id="9fac2-113">[Read the ADAL FAQ](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span></span>
1. <span data-ttu-id="9fac2-114">[Saznajte kako da migrirate aplikacije na osnovu osnove po platformoji](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span><span class="sxs-lookup"><span data-stu-id="9fac2-114">[Learn about how to migrate apps on a per-platform basis](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).</span></span>
1. <span data-ttu-id="9fac2-115">Ako vam je potrebna pomoć da biste razumeli koje aplikacije koriste ADALE, preporučujemo da pregledate sve izvorne kodove za aplikacije i ako je to primenljivo, da pristupite bilo kom dobavljaču ili dobavljačima aplikacija.</span><span class="sxs-lookup"><span data-stu-id="9fac2-115">If you need help understanding which of your apps use ADAL, we recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="9fac2-116">Microsoft podrška vam takođe može pružiti listu svih aplikacija koje ne podržavaju Microsoft u vašem zakupcu.</span><span class="sxs-lookup"><span data-stu-id="9fac2-116">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>

<span data-ttu-id="9fac2-117">**AAD Graph migracija**</span><span class="sxs-lookup"><span data-stu-id="9fac2-117">**AAD Graph Migration**</span></span>

<span data-ttu-id="9fac2-118">Za aplikacije koje koriste Azure AD Graph, potražite uputstvo za migraciju [AZURE AD Graph grafika u Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview?view=graph-rest-1.0&preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="9fac2-118">For applications that are using Azure AD Graph, follow our guidance to migrate [Azure AD Graph apps to Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview?view=graph-rest-1.0&preserve-view=true).</span></span>

1. <span data-ttu-id="9fac2-119">[Naša kontrolna lista za migraciju pruža taиku na početku](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span><span class="sxs-lookup"><span data-stu-id="9fac2-119">[Our migration checklist provides a getting started point](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span></span> 
1. <span data-ttu-id="9fac2-120">Vaš Azure registracioni portal pokazuje koje aplikacije koriste AAD Graph.</span><span class="sxs-lookup"><span data-stu-id="9fac2-120">Your Azure app registration portal shows which applications are using AAD Graph.</span></span> <span data-ttu-id="9fac2-121">Preporučujemo da pregledate sve izvorne kodove za aplikacije i ako je to primenljivo, da pristupite bilo kom dobavljaču ili dobavljačima aplikacija.</span><span class="sxs-lookup"><span data-stu-id="9fac2-121">We recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="9fac2-122">Microsoft podrška vam takođe može pružiti listu svih podrške za AAD Graph u zakupcu.</span><span class="sxs-lookup"><span data-stu-id="9fac2-122">Microsoft support can also provide you with a list of all AAD Graph usage in your tenant.</span></span>
1. <span data-ttu-id="9fac2-123">Da bi aplikacija pristupala podacima u programu Microsoft Graph, korisnik ili administrator mora da joj dodeli ispravne dozvole putem procesa pristanka.</span><span class="sxs-lookup"><span data-stu-id="9fac2-123">For your app to access data in Microsoft Graph, the user or administrator must grant it the correct permissions via a consent process.</span></span> <span data-ttu-id="9fac2-124">[Referenca sa Microsoft Graph dozvolama](https://docs.microsoft.com/graph/permissions-reference?context=graph%2Fapi%2Fbeta&view=graph-rest-beta&preserve-view=true) navodi dozvole povezane sa svakim glavnim skupom Microsoft Graph API.</span><span class="sxs-lookup"><span data-stu-id="9fac2-124">The [Microsoft Graph permissions reference](https://docs.microsoft.com/graph/permissions-reference?context=graph%2Fapi%2Fbeta&view=graph-rest-beta&preserve-view=true) lists the permissions associated with each major set of Microsoft Graph APIs.</span></span> <span data-ttu-id="9fac2-125">On takođe pruža uputstva o tome kako da koristite dozvole.</span><span class="sxs-lookup"><span data-stu-id="9fac2-125">It also provides guidance about how to use the permissions.</span></span>
