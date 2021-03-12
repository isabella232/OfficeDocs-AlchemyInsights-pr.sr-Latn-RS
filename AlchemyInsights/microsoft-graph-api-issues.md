---
title: Problemi sa Microsoft Graph API-om
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
- "9004345"
- "7759"
ms.openlocfilehash: a856094d9152568c3c067da5856153230d6590a6
ms.sourcegitcommit: 9d03083ea6e18070296b87a1b02339ca4d8e6064
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 01/29/2021
ms.locfileid: "50714158"
---
# <a name="microsoft-graph-api-issues"></a><span data-ttu-id="aa295-102">Problemi sa Microsoft Graph API-om</span><span class="sxs-lookup"><span data-stu-id="aa295-102">Microsoft Graph API issues</span></span>

<span data-ttu-id="aa295-103">Ova tema može da se primenjuje i na programere koji i dalje koriste Azure AD Graph Graf.</span><span class="sxs-lookup"><span data-stu-id="aa295-103">This topic may also apply to developers still using Azure AD Graph API.</span></span> <span data-ttu-id="aa295-104">Međutim **, preporučuje se** da koristite Microsoft Graph za sve kataloge, identitete i Access scenarije upravljanja pristupom.</span><span class="sxs-lookup"><span data-stu-id="aa295-104">However, it is **strongly** recommended that you use Microsoft Graph for all your directory, identity, and access management scenarios.</span></span>

<span data-ttu-id="aa295-105">**Problemi sa autentikacijom ili autorizacijom**</span><span class="sxs-lookup"><span data-stu-id="aa295-105">**Authentication or authorization issues**</span></span>

- <span data-ttu-id="aa295-106">Ako aplikacija **ne može da dobije simbole** da bi pozvala Microsoft Graph, odaberite **problem sa prilikom dobijanja simbola za pristup (potvrda identiteta)** Microsoft Graph da bi se pribavila preciznije pomoć i podrška na ovoj temi.</span><span class="sxs-lookup"><span data-stu-id="aa295-106">If your app is **unable to acquire tokens** to call Microsoft Graph, pick **Problem with getting an access token (Authentication)** Microsoft Graph category to get more specific help and support on this topic.</span></span>
- <span data-ttu-id="aa295-107">Ako aplikacija **prima 401 ili 403 greške autorizacije** prilikom pozivanja Microsoft dijagrama, izaberite kategoriju " **Preuzimanje zabrane pristupa" (autorizacija)** Microsoft Graph API za dobijanje specifične pomoći i podrške u ovoj temi.</span><span class="sxs-lookup"><span data-stu-id="aa295-107">If your app is **receiving 401 or 403 authorization errors** when calling Microsoft Graph, pick the **Getting an access denied error (Authorization)** Microsoft Graph API category to get more specific help and support on this topic.</span></span>

<span data-ttu-id="aa295-108">**Želim da koristim Microsoft Graph, ali ne znam gde da počnem**</span><span class="sxs-lookup"><span data-stu-id="aa295-108">**I want to use Microsoft Graph, but not sure where to start**</span></span>

- [<span data-ttu-id="aa295-109">Pregled programa Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="aa295-109">Overview of Microsoft Graph</span></span>](https://docs.microsoft.com/graph/overview)
- [<span data-ttu-id="aa295-110">Pregled identiteta i upravljanja pristupom u programu Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="aa295-110">Overview of Identity and Access Management in Microsoft Graph</span></span>](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [<span data-ttu-id="aa295-111">Prvi koraci u pravljenju Microsoft Graph aplikacija</span><span class="sxs-lookup"><span data-stu-id="aa295-111">Getting started building Microsoft Graph apps</span></span>](https://docs.microsoft.com/graph/)
- <span data-ttu-id="aa295-112">**Microsoft Graph Explorer** – testiranje Microsoft Graph API-ja u zakupcu ili na demo zakupcu</span><span class="sxs-lookup"><span data-stu-id="aa295-112">**Microsoft Graph Explorer** - Test Microsoft Graph APIs in your tenant or a demo tenant</span></span>

<span data-ttu-id="aa295-113">**Želim da koristim Microsoft Graph, ali da li podržava API-ju usluge v 1.0?**</span><span class="sxs-lookup"><span data-stu-id="aa295-113">**I want to use Microsoft Graph, but does it support the v1.0 directory APIs I need?**</span></span>

<span data-ttu-id="aa295-114">Microsoft Graph je preporučeni API za upravljanje katalogom, identitetom i Access upravljanju.</span><span class="sxs-lookup"><span data-stu-id="aa295-114">Microsoft Graph is the recommended API for directory, identity, and access management.</span></span> <span data-ttu-id="aa295-115">Međutim, postoji nekoliko razmaka između onoga što je moguće u usluzi Azure A.D. i Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="aa295-115">However, there are still a few gaps between what is possible in Azure AD Graph and Microsoft Graph.</span></span> <span data-ttu-id="aa295-116">Pregledajte sledeće članke koji naglašavaju najnovije razlike koje će vam pomoći u izboru:</span><span class="sxs-lookup"><span data-stu-id="aa295-116">Review the following articles, which highlight the most up-to-date differences to assist in your choice:</span></span>

- [<span data-ttu-id="aa295-117">Razlike tipa resursa između Azure reklama i Microsoft dijagrama</span><span class="sxs-lookup"><span data-stu-id="aa295-117">Resource type differences between Azure AD Graph and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [<span data-ttu-id="aa295-118">Razlike u svojstvima između Azure A.D. Grafa i Microsoft dijagrama</span><span class="sxs-lookup"><span data-stu-id="aa295-118">Property differences between Azure AD Graph and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [<span data-ttu-id="aa295-119">Razlike metoda između Azure AD i Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="aa295-119">Method differences between Azure AD and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

<span data-ttu-id="aa295-120">**API koji zovem ne radi-gde mogu da uradim više testiranja?**</span><span class="sxs-lookup"><span data-stu-id="aa295-120">**The API I am calling doesn't work - where can I do more testing?**</span></span>

<span data-ttu-id="aa295-121">**Microsoft Graph Explorer** – testiranje Microsoft Graph API-ja u zakupcu ili na demonstracijuzakupcu i pročitajte **probne upite** u programu Microsoft Graph Explorer.</span><span class="sxs-lookup"><span data-stu-id="aa295-121">**Microsoft Graph Explorer** - Test Microsoft Graph APIs in your tenant or a demo tenant and also check out the **sample queries** in Microsoft Graph Explorer.</span></span>

<span data-ttu-id="aa295-122">**Moja aplikacija je prespora i takođe se koristi. Koja poboljšanja mogu da napravim?**</span><span class="sxs-lookup"><span data-stu-id="aa295-122">**My app is too slow and is also getting throttled. What improvements can I make?**</span></span>

<span data-ttu-id="aa295-123">U zavisnosti od scenarija, postoji mnoštvo opcija koje vam pripadaju na raspolaganju da biste aplikaciju načinili pristupačnijim, a u nekoliko slučajeva, manje sklon odbacivanjem usluge (kada pravite previše poziva).</span><span class="sxs-lookup"><span data-stu-id="aa295-123">Depending on your scenario, there are a variety of options at your disposal to make your application more performant, and in some cases, less prone to being throttled by the service (when you are making too many calls).</span></span>

- [<span data-ttu-id="aa295-124">Najbolje prakse za Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="aa295-124">Microsoft Graph best practices</span></span>](https://docs.microsoft.com/graph/best-practices-concept)
- [<span data-ttu-id="aa295-125">Zahtevi za sastanak</span><span class="sxs-lookup"><span data-stu-id="aa295-125">Batching requests</span></span>](https://docs.microsoft.com/graph/json-batching)
- [<span data-ttu-id="aa295-126">Praćenje promena kroz Delta Query</span><span class="sxs-lookup"><span data-stu-id="aa295-126">Track changes through delta query</span></span>](https://docs.microsoft.com/graph/delta-query-overview)
- [<span data-ttu-id="aa295-127">Obaveštenje o promenama pomoću Veb-udica</span><span class="sxs-lookup"><span data-stu-id="aa295-127">Get notified of changes through webhooks</span></span>](https://docs.microsoft.com/graph/webhooks)
- [<span data-ttu-id="aa295-128">Usmeravanje smernica</span><span class="sxs-lookup"><span data-stu-id="aa295-128">Throttling guidance</span></span>](https://docs.microsoft.com/graph/throttling)

<span data-ttu-id="aa295-129">**Gde mogu da pronađem više informacija o greškama i poznatim problemima?**</span><span class="sxs-lookup"><span data-stu-id="aa295-129">**Where can I find more information on errors and known issues?**</span></span>

- [<span data-ttu-id="aa295-130">Informacije o odgovoru na Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="aa295-130">Microsoft Graph error response information</span></span>](https://docs.microsoft.com/graph/errors)
- [<span data-ttu-id="aa295-131">Poznati problemi sa programom Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="aa295-131">Known issues with Microsoft Graph</span></span>](https://docs.microsoft.com/graph/known-issues)

<span data-ttu-id="aa295-132">**Gde mogu da proverim status raspoloživost usluge i vezu?**</span><span class="sxs-lookup"><span data-stu-id="aa295-132">**Where can I check status of service availability and connectivity?**</span></span>

<span data-ttu-id="aa295-133">Raspoloživost usluge i veza osnovnih usluga kojima se može pristupiti pomoću programa Microsoft Graph može da utiče na ukupnu dostupnost i performanse programa Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="aa295-133">The service availability and connectivity of the underlying services that can be accessed through Microsoft Graph can impact the overall availability and performance of Microsoft Graph.</span></span>

- <span data-ttu-id="aa295-134">Za Azure Active Directory zdravstveni sistem, potvrdite status **bezbednosti + usluge identiteta** navedenih na [stranici Azure status](https://azure.microsoft.com/status/).</span><span class="sxs-lookup"><span data-stu-id="aa295-134">For Azure Active Directory service health, check the status of **Security + Identity** services listed in the [Azure status page](https://azure.microsoft.com/status/).</span></span>
- <span data-ttu-id="aa295-135">Za Office usluge koje doprinose programu Microsoft Graph, potvrdite status usluga navedenim na [kontrolnoj tabli usluge Office usluga](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="aa295-135">For Office services that contribute to Microsoft Graph, check the status of services listed in the [Office Service Health Dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>

<span data-ttu-id="aa295-136">Greške Microsoft Graph autorizacije mogu da budu rezultat nekoliko raznih problema, od kojih većina stvara 401 ili 403 grešku.</span><span class="sxs-lookup"><span data-stu-id="aa295-136">Microsoft Graph authorization errors can be a result of several different issues, most of which generate a 401 or 403 error.</span></span> <span data-ttu-id="aa295-137">Na primer, sledeće mogu sve da dovedu do grešaka autorizacije:</span><span class="sxs-lookup"><span data-stu-id="aa295-137">For example, the following can all lead to authorization errors:</span></span>

- <span data-ttu-id="aa295-138">Neispravno [tokovi prikupljanja tokena za pristup](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-scenarios)</span><span class="sxs-lookup"><span data-stu-id="aa295-138">Incorrect [access token acquisition flows](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-scenarios)</span></span>
- <span data-ttu-id="aa295-139">Loše konfigurisani[opsezi dozvola](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes)</span><span class="sxs-lookup"><span data-stu-id="aa295-139">Poorly configured [permission scopes](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes)</span></span>
- <span data-ttu-id="aa295-140">Nedostatak [pristanka](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)</span><span class="sxs-lookup"><span data-stu-id="aa295-140">Lack of [consent](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)</span></span>

<span data-ttu-id="aa295-141">\**_Kraj podrške za Azure Active Directory biblioteku potvrde identiteta (ADAL) i Azure AD Graph API (AAD Graph)_* _</span><span class="sxs-lookup"><span data-stu-id="aa295-141">\**_End of support for Azure Active Directory Authentication Library (ADAL) and Azure AD Graph API (AAD Graph)_* _</span></span>

<span data-ttu-id="aa295-142"># \* Počevši od 30 juna, 2020 \* \*, više nećemo dodavati nove funkcije u ADALE i Azure AD Graph.</span><span class="sxs-lookup"><span data-stu-id="aa295-142">_\*Starting June 30th, 2020\*\*, we will no longer add any new features to ADAL and Azure AD Graph.</span></span> <span data-ttu-id="aa295-143">Nastavićemo da pružamo tehničku podršku i bezbednosne ispravke, ali više nećemo pružati ispravke funkcija.</span><span class="sxs-lookup"><span data-stu-id="aa295-143">We will continue to provide technical support and security updates but will no longer provide feature updates.</span></span>

<span data-ttu-id="aa295-144">**Počevši od 30 juna, 2022**, završićemo podršku za Adale i AZURE AD Graf i neće više pružiti tehničku podršku ili bezbednosne ispravke.</span><span class="sxs-lookup"><span data-stu-id="aa295-144">**Starting June 30th, 2022**, we will end support for ADAL and Azure AD Graph and will no longer provide technical support or security updates.</span></span>

<span data-ttu-id="aa295-145">Aplikacije koje koriste ADAL na postojećim verzijama OS nastaviće da funkcionišu posle ovog vremena, ali neće *dobiti tehničku podršku ili bezbednosne ispravke*.</span><span class="sxs-lookup"><span data-stu-id="aa295-145">Apps using ADAL on existing OS versions will continue to work after this time but will not *get any technical support or security updates*.</span></span>

<span data-ttu-id="aa295-146">Aplikacije koje koriste Azure AD Graph posle ovog vremena možda više neće primati odgovore od krajnje tačke Azure oglasa Graph.</span><span class="sxs-lookup"><span data-stu-id="aa295-146">Apps using Azure AD Graph after this time may no longer receive responses from the Azure AD Graph endpoint.</span></span>

<span data-ttu-id="aa295-147">**ADALA migracija**</span><span class="sxs-lookup"><span data-stu-id="aa295-147">**ADAL Migration**</span></span>

<span data-ttu-id="aa295-148">Preporučujemo ažuriranje na [Microsoft Authentication Library (MSAL) ](https://docs.microsoft.com/azure/active-directory/develop/v2-overview)koja ima najnovije funkcije i bezbednosne ispravke.</span><span class="sxs-lookup"><span data-stu-id="aa295-148">We recommend updating to the [Microsoft Authentication Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), which has the latest features and security updates.</span></span>

<span data-ttu-id="aa295-149">Ako koristite Microsoft aplikacije, znajte da je Microsoft u procesu migriranja svojih aplikacija u MSAL pomoću krajnjeg roka za podršku, kada se osigura da će imati koristi od msalove trenutne bezbednosti i poboljšanja funkcija.</span><span class="sxs-lookup"><span data-stu-id="aa295-149">If you are using Microsoft apps, know that Microsoft is in the process of migrating its applications to MSAL by the end-of-support deadline, ensuring they'll benefit from MSAL's ongoing security and feature improvements.</span></span>

1. [<span data-ttu-id="aa295-150">Pročitajte najčešća pitanja za ADAL</span><span class="sxs-lookup"><span data-stu-id="aa295-150">Read the ADAL FAQ</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [<span data-ttu-id="aa295-151">Saznajte više o tome kako da migrirate aplikacije na osnovu platforme</span><span class="sxs-lookup"><span data-stu-id="aa295-151">Learn about how to migrate apps on a per-platform basis</span></span>](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. <span data-ttu-id="aa295-152">Ako vam je potrebna pomoć da biste razumeli koje aplikacije koriste ADALE, preporučujemo da pregledate sve izvorne kodove za aplikacije i ako je to primenljivo, da pristupite bilo kom dobavljaču ili dobavljačima aplikacija.</span><span class="sxs-lookup"><span data-stu-id="aa295-152">If you need help understanding which of your apps use ADAL, we recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="aa295-153">Microsoft podrška vam takođe može pružiti listu svih aplikacija koje nisu Microsoft ADAL u vašem zakupcu.</span><span class="sxs-lookup"><span data-stu-id="aa295-153">Microsoft support can also provide you with a list of all non-Microsoft ADAL apps in your tenant.</span></span>

<span data-ttu-id="aa295-154">**AAD Graph migracija**</span><span class="sxs-lookup"><span data-stu-id="aa295-154">**AAD Graph Migration**</span></span>

<span data-ttu-id="aa295-155">Za aplikacije koje koriste Azure AD Graph, potražite uputstvo za [migraciju AZURE AD Graph grafika u Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview).</span><span class="sxs-lookup"><span data-stu-id="aa295-155">For applications that are using Azure AD Graph, follow our guidance to [migrate Azure AD Graph apps to Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview).</span></span>

1. <span data-ttu-id="aa295-156">[Naša lista za migraciju pruža tačku za početak](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span><span class="sxs-lookup"><span data-stu-id="aa295-156">[Our migration checklist provides a getting started point](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).</span></span>
2. <span data-ttu-id="aa295-157">Vaš portal za registraciju aplikacija Azure prikazuje koje aplikacije koriste AAD Graph.</span><span class="sxs-lookup"><span data-stu-id="aa295-157">Your Azure app registration portal shows which applications are using AAD Graph.</span></span> <span data-ttu-id="aa295-158">Preporučujemo vam da pregledate sav izvorni kod aplikacija i, ako je primenljivo, kontaktirate bilo koje ISV-ove ili dobavljače aplikacija.</span><span class="sxs-lookup"><span data-stu-id="aa295-158">We recommend you review all of your apps' source code, and if applicable, reach out to any ISVs or app providers.</span></span> <span data-ttu-id="aa295-159">Microsoft podrška vam takođe može pružiti listu svih podrške za AAD Graph u zakupcu.</span><span class="sxs-lookup"><span data-stu-id="aa295-159">Microsoft support can also provide you with a list of all AAD Graph usage in your tenant.</span></span>
3. <span data-ttu-id="aa295-160">Da bi aplikacija pristupala podacima u programu Microsoft Graph, korisnik ili administrator mora da joj dodeli ispravne dozvole putem procesa pristanka.</span><span class="sxs-lookup"><span data-stu-id="aa295-160">For your app to access data in Microsoft Graph, the user or administrator must grant it the correct permissions via a consent process.</span></span> <span data-ttu-id="aa295-161">[Referenca sa Microsoft Graph dozvolama](https://docs.microsoft.com/graph/permissions-reference) navodi dozvole povezane sa svakim glavnim skupom Microsoft Graph API.</span><span class="sxs-lookup"><span data-stu-id="aa295-161">The [Microsoft Graph permissions reference](https://docs.microsoft.com/graph/permissions-reference) lists the permissions associated with each major set of Microsoft Graph APIs.</span></span> <span data-ttu-id="aa295-162">On takođe pruža uputstva o tome kako da koristite dozvole.</span><span class="sxs-lookup"><span data-stu-id="aa295-162">It also provides guidance about how to use the permissions.</span></span>
