---
title: Izvršavanje upita prema Microsoft Graph API
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
- "7846"
ms.openlocfilehash: 527e88c7b3cb1cc4f5535e3b0d2bc4d8d1163336
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974684"
---
# <a name="querying-the-microsoft-graph-api"></a><span data-ttu-id="924f2-102">Izvršavanje upita prema Microsoft Graph API</span><span class="sxs-lookup"><span data-stu-id="924f2-102">Querying the Microsoft Graph API</span></span>

<span data-ttu-id="924f2-103">Ova tema može da se primenjuje i na programere koji i dalje koriste Azure AD Graph Graf.</span><span class="sxs-lookup"><span data-stu-id="924f2-103">This topic may also apply to developers still using Azure AD Graph API.</span></span> <span data-ttu-id="924f2-104">Međutim **, preporučuje se** da koristite Microsoft Graph za sve kataloge, identitete i Access scenarije upravljanja pristupom.</span><span class="sxs-lookup"><span data-stu-id="924f2-104">However, it is **strongly** recommended that you use Microsoft Graph for all your directory, identity, and access management scenarios.</span></span>

<span data-ttu-id="924f2-105">**Problemi sa autentikacijom ili autorizacijom**</span><span class="sxs-lookup"><span data-stu-id="924f2-105">**Authentication or authorization issues**</span></span>

- <span data-ttu-id="924f2-106">Ako aplikacija **ne može da dobije simbole** da bi pozvala Microsoft Graph, odaberite **problem sa prilikom dobijanja simbola za pristup (potvrda identiteta)** Microsoft Graph da bi se pribavila preciznije pomoć i podrška na ovoj temi.</span><span class="sxs-lookup"><span data-stu-id="924f2-106">If your app is **unable to acquire tokens** to call Microsoft Graph, pick **Problem with getting an access token (Authentication)** Microsoft Graph category to get more specific help and support on this topic.</span></span>
- <span data-ttu-id="924f2-107">Ako aplikacija **prima 401 ili 403 greške autorizacije** prilikom pozivanja Microsoft dijagrama, izaberite kategoriju " **Preuzimanje zabrane pristupa" (autorizacija)** Microsoft Graph API za dobijanje specifične pomoći i podrške u ovoj temi.</span><span class="sxs-lookup"><span data-stu-id="924f2-107">If your app is **receiving 401 or 403 authorization errors** when calling Microsoft Graph, pick the **Getting an access denied error (Authorization)** Microsoft Graph API category to get more specific help and support on this topic.</span></span>

<span data-ttu-id="924f2-108">**Želim da koristim Microsoft Graph, ali ne znam gde da počnem**</span><span class="sxs-lookup"><span data-stu-id="924f2-108">**I want to use Microsoft Graph, but not sure where to start**</span></span>

<span data-ttu-id="924f2-109">Da biste saznali više o programu Microsoft Graph, pogledajte:</span><span class="sxs-lookup"><span data-stu-id="924f2-109">To learn more about Microsoft Graph, see:</span></span>

- [<span data-ttu-id="924f2-110">Pregled programa Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="924f2-110">Overview of Microsoft Graph</span></span>](https://docs.microsoft.com/graph/overview)
- [<span data-ttu-id="924f2-111">Pregled identiteta i upravljanja pristupom u programu Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="924f2-111">Overview of Identity and Access Management in Microsoft Graph</span></span>](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [<span data-ttu-id="924f2-112">Prvi koraci u pravljenju Microsoft Graph aplikacija</span><span class="sxs-lookup"><span data-stu-id="924f2-112">Getting started building Microsoft Graph apps</span></span>](https://docs.microsoft.com/graph/)
- <span data-ttu-id="924f2-113">**Microsoft Graph Explorer** – testiranje Microsoft Graph API-ja u zakupcu ili na demo zakupcu</span><span class="sxs-lookup"><span data-stu-id="924f2-113">**Microsoft Graph Explorer** - Test Microsoft Graph APIs in your tenant or a demo tenant</span></span>

<span data-ttu-id="924f2-114">**Želim da koristim Microsoft Graph, ali da li podržava API-ju usluge v 1.0?**</span><span class="sxs-lookup"><span data-stu-id="924f2-114">**I want to use Microsoft Graph, but does it support the v1.0 directory APIs I need?**</span></span>

<span data-ttu-id="924f2-115">Microsoft Graph je preporučeni API za upravljanje katalogom, identitetom i Access upravljanju.</span><span class="sxs-lookup"><span data-stu-id="924f2-115">Microsoft Graph is the recommended API for directory, identity, and access management.</span></span> <span data-ttu-id="924f2-116">Međutim, postoji nekoliko razmaka između onoga što je moguće u usluzi Azure A.D. i Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="924f2-116">However, there are still a few gaps between what is possible in Azure AD Graph and Microsoft Graph.</span></span> <span data-ttu-id="924f2-117">Pregledajte sledeće članke koji naglašavaju najnovije razlike koje će vam pomoći u izboru:</span><span class="sxs-lookup"><span data-stu-id="924f2-117">Review the following articles, which highlight the most up-to-date differences to assist in your choice:</span></span>

- [<span data-ttu-id="924f2-118">Razlike tipa resursa između Azure reklama i Microsoft dijagrama</span><span class="sxs-lookup"><span data-stu-id="924f2-118">Resource type differences between Azure AD Graph and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [<span data-ttu-id="924f2-119">Razlike u svojstvima između Azure A.D. Grafa i Microsoft dijagrama</span><span class="sxs-lookup"><span data-stu-id="924f2-119">Property differences between Azure AD Graph and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [<span data-ttu-id="924f2-120">Razlike metoda između Azure AD i Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="924f2-120">Method differences between Azure AD and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

<span data-ttu-id="924f2-121">**Kada upitim *korisnički* objekat, mnoga svojstva nedostaju**</span><span class="sxs-lookup"><span data-stu-id="924f2-121">**When I query the *user* object, many of its properties are missing**</span></span>

<span data-ttu-id="924f2-122">`GET https://graph.microsoft.com/v1.0/users` daje samo 11 svojstava, kao što Microsoft Graph automatski bira podrazumevani skupa svojstava *korisnika* .</span><span class="sxs-lookup"><span data-stu-id="924f2-122">`GET https://graph.microsoft.com/v1.0/users` only returns 11 properties, as Microsoft Graph auto-selects a default set of *user* properties to return.</span></span> <span data-ttu-id="924f2-123">Ako su vam potrebna i druga svojstva *korisnika* , koristite $SELECT da biste izabrali svojstva koja su vam potrebna.</span><span class="sxs-lookup"><span data-stu-id="924f2-123">If you need other *user* properties, use $select to pick the properties your application needs.</span></span> <span data-ttu-id="924f2-124">Prvo isprobajte **Microsoft Graph Explorer** .</span><span class="sxs-lookup"><span data-stu-id="924f2-124">Try it out in **Microsoft Graph Explorer** first.</span></span>

<span data-ttu-id="924f2-125">**Neke vrednosti korisničkog vlasništva su *Null* iako znam da su podešene**</span><span class="sxs-lookup"><span data-stu-id="924f2-125">**Some user property values are *null* even though I know they are set**</span></span>

<span data-ttu-id="924f2-126">Najverovatnije objašnjenje je da je aplikaciji dodeljena *Korisnička. ReadBasic. sva* dozvola.</span><span class="sxs-lookup"><span data-stu-id="924f2-126">The most likely explanation is that the application had been granted the *User.ReadBasic.All* permission.</span></span> <span data-ttu-id="924f2-127">To omogućava aplikaciji da čita ograničeni broj svojstava korisnika, vraća sva druga svojstva kao NULL, čak i ako su prethodno podešene.</span><span class="sxs-lookup"><span data-stu-id="924f2-127">This allows the application to read a limited set of user properties, returning all other properties as null even if they have been previously set.</span></span> <span data-ttu-id="924f2-128">Isprobajte *korisniku aplikacije. pročitajte. sve* dozvole.</span><span class="sxs-lookup"><span data-stu-id="924f2-128">Try granting the application *User.Read.All* permission instead.</span></span>

<span data-ttu-id="924f2-129">Više informacija potražite u članku [dozvole za Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference#user-permissions).</span><span class="sxs-lookup"><span data-stu-id="924f2-129">For more information, see [Microsoft Graph user permissions](https://docs.microsoft.com/graph/permissions-reference#user-permissions).</span></span>

<span data-ttu-id="924f2-130">**Imam problema sa korišćenjem OData parametara upita za filtriranje podataka u svojim zahtevima**</span><span class="sxs-lookup"><span data-stu-id="924f2-130">**I'm having trouble using OData query parameters to filter data in my requests**</span></span>

<span data-ttu-id="924f2-131">Dok Microsoft Graph podržava širok opseg parametara OData upita, mnogi od tih parametara nisu u potpunosti podržani od strane usluga direktorijuma (resursi koji nasleđuju od *Directoryobject*) u programu Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="924f2-131">While Microsoft Graph supports a wide range of the OData query parameters, many of those parameters are not fully supported by directory services (resources that inherit from *directoryObject*) in Microsoft Graph.</span></span> <span data-ttu-id="924f2-132">Ista ograničenja koja su bila prisutan u usluzi Azure AD Graph se i dalje najčešće nalaze u programu Microsoft Graph:</span><span class="sxs-lookup"><span data-stu-id="924f2-132">The same limitations that were present in Azure AD Graph persist for the most part in Microsoft Graph:</span></span>

1. <span data-ttu-id="924f2-133">**Nije podržano**: $count, $search i $filter u vrednostima *Null* ili *Ne bez* vrednosti</span><span class="sxs-lookup"><span data-stu-id="924f2-133">**Not supported**: $count, $search, and $filter on *null* or *not null* values</span></span>
2. <span data-ttu-id="924f2-134">**Nije podržano**: $filter na određenim svojstvima (pogledajte teme za resurse na kojima su svojstva filtriena)</span><span class="sxs-lookup"><span data-stu-id="924f2-134">**Not supported**: $filter on certain properties (see resource topics on which properties are filterable)</span></span>
3. <span data-ttu-id="924f2-135">**Nije podržano**: istovremeno stranične memorije, filtriranje i sortiranje</span><span class="sxs-lookup"><span data-stu-id="924f2-135">**Not supported**: paging, filtering, and sorting at the same time</span></span>
4. <span data-ttu-id="924f2-136">**Nije podržano**: filtriranje relacije.</span><span class="sxs-lookup"><span data-stu-id="924f2-136">**Not supported**: filtering on a relationship.</span></span> <span data-ttu-id="924f2-137">Na primer – pronađite sve članove inženjerske grupe koji se nalaze u Britaniji.</span><span class="sxs-lookup"><span data-stu-id="924f2-137">For example - find all members of the engineering group that are in the UK.</span></span>
5. <span data-ttu-id="924f2-138">**Delimična podrška**: $OrderBy na *korisničkom* (Displayime i userprincipalime) i *grupi*</span><span class="sxs-lookup"><span data-stu-id="924f2-138">**Partial support**: $orderby on *user* (displayName and userPrincipalName only) and *group*</span></span>
6. <span data-ttu-id="924f2-139">**Delimična podrška**: $filter (podržava samo *EQ*, *startswith*, *ili*, *i* ograničeno *bilo koja*) podrška, $Expand (proširivanje relacija jednog objekta vraća sve relacije, ali proširenje relacija objekata se ograničava)</span><span class="sxs-lookup"><span data-stu-id="924f2-139">**Partial support**: $filter (supports only *eq*, *startswith*, *or*, *and*, and limited *any*) support, $expand (expanding a single object's relationships returns all relationships, but expanding a collection of objects' relationships is limited)</span></span>

<span data-ttu-id="924f2-140">Više informacija potražite u članku [Prilagođavanje odgovora pomoću parametara upita](https://docs.microsoft.com/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="924f2-140">For more information, see [Customize responses with query parameters](https://docs.microsoft.com/graph/query-parameters).</span></span>

<span data-ttu-id="924f2-141">**API koji zovem ne radi-gde mogu da uradim više testiranja?**</span><span class="sxs-lookup"><span data-stu-id="924f2-141">**The API I'm calling doesn't work - where can I do more testing?**</span></span>

<span data-ttu-id="924f2-142">**Microsoft Graph Explorer** – testiranje Microsoft Graph API-ja u zakupcu ili na demonstracijuzakupcu i pročitajte **probne upite** u programu Microsoft Graph Explorer.</span><span class="sxs-lookup"><span data-stu-id="924f2-142">**Microsoft Graph Explorer** - Test Microsoft Graph APIs in your tenant or a demo tenant and also check out the **sample queries** in Microsoft Graph Explorer.</span></span>

<span data-ttu-id="924f2-143">**Kada upitim za podatke, čini se da dobijam nazad nepotpun skupa podataka**</span><span class="sxs-lookup"><span data-stu-id="924f2-143">**When I query for data it seems like I get an incomplete data set back**</span></span>

<span data-ttu-id="924f2-144">Ako upitate kolekciju (kao što su *Korisnici*), Microsoft Graph koristi ograničenja stranice servera tako da se rezultati uvek vraćaju sa podrazumevanom veličinom stranice.</span><span class="sxs-lookup"><span data-stu-id="924f2-144">If you are querying a collection (like *users*), Microsoft Graph uses server-side page limits so results are always returned with a default page-size.</span></span> <span data-ttu-id="924f2-145">Aplikacija bi uvek trebalo da očekuje da stranica kroz kolekcije vrati iz usluge.</span><span class="sxs-lookup"><span data-stu-id="924f2-145">Your app should always expect to page through collections returned from the service.</span></span>

<span data-ttu-id="924f2-146">Za više informacija pogledajte članak:</span><span class="sxs-lookup"><span data-stu-id="924f2-146">For more information, see:</span></span>

- [<span data-ttu-id="924f2-147">Najbolje prakse za Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="924f2-147">Microsoft Graph best practices</span></span>](https://docs.microsoft.com/graph/best-practices-concept)
- [<span data-ttu-id="924f2-148">Stranične memorije za Microsoft Graph u aplikaciji</span><span class="sxs-lookup"><span data-stu-id="924f2-148">Paging Microsoft Graph data in your app</span></span>](https://docs.microsoft.com/graph/paging)

<span data-ttu-id="924f2-149">**Moja aplikacija je prespora i takođe se koristi. Koja poboljšanja mogu da napravim?**</span><span class="sxs-lookup"><span data-stu-id="924f2-149">**My app is too slow and is also getting throttled. What improvements can I make?**</span></span>

<span data-ttu-id="924f2-150">U zavisnosti od scenarija, postoji mnoštvo različitih opcija koje su vam na raspolaganju da bi aplikacija bila pristupačnija, a u nekoliko slučajeva, manje sklona odbacivanju od strane usluge (kada pravite previše poziva).</span><span class="sxs-lookup"><span data-stu-id="924f2-150">Depending on your scenario, there are a variety of different options at your disposal to make your application more performant, and in some cases, less prone to being throttled by the service (when you are making too many calls).</span></span>

<span data-ttu-id="924f2-151">Više informacija potražite u sledećim člancima:</span><span class="sxs-lookup"><span data-stu-id="924f2-151">To learn more, see:</span></span>

- [<span data-ttu-id="924f2-152">Najbolje prakse za Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="924f2-152">Microsoft Graph best practices</span></span>](https://docs.microsoft.com/graph/best-practices-concept)
- [<span data-ttu-id="924f2-153">Zahtevi za sastanak</span><span class="sxs-lookup"><span data-stu-id="924f2-153">Batching requests</span></span>](https://docs.microsoft.com/graph/json-batching)
- [<span data-ttu-id="924f2-154">Praćenje promena kroz Delta Query</span><span class="sxs-lookup"><span data-stu-id="924f2-154">Track changes through delta query</span></span>](https://docs.microsoft.com/graph/delta-query-overview)
- [<span data-ttu-id="924f2-155">Obaveštenje o promenama pomoću Veb-udica</span><span class="sxs-lookup"><span data-stu-id="924f2-155">Get notified of changes through webhooks</span></span>](https://docs.microsoft.com/graph/webhooks)
- [<span data-ttu-id="924f2-156">Usmeravanje smernica</span><span class="sxs-lookup"><span data-stu-id="924f2-156">Throttling guidance</span></span>](https://docs.microsoft.com/graph/throttling)

<span data-ttu-id="924f2-157">**Gde mogu da pronađem više informacija o greškama i poznatim problemima?**</span><span class="sxs-lookup"><span data-stu-id="924f2-157">**Where can I find more information on errors and known issues?**</span></span>

- [<span data-ttu-id="924f2-158">Informacije o odgovoru na Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="924f2-158">Microsoft Graph error response information</span></span>](https://docs.microsoft.com/graph/errors)
- [<span data-ttu-id="924f2-159">Poznati problemi sa programom Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="924f2-159">Known issues with Microsoft Graph</span></span>](https://docs.microsoft.com/graph/known-issues)

<span data-ttu-id="924f2-160">**Gde mogu da proverim status raspoloživost usluge i vezu?**</span><span class="sxs-lookup"><span data-stu-id="924f2-160">**Where can I check status of service availability and connectivity?**</span></span>

<span data-ttu-id="924f2-161">Raspoloživost usluge i veza osnovnih usluga kojima se može pristupiti pomoću programa Microsoft Graph može da utiče na ukupnu dostupnost i performanse programa Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="924f2-161">The service availability and connectivity of the underlying services that can be accessed through Microsoft Graph can impact the overall availability and performance of Microsoft Graph.</span></span>

- <span data-ttu-id="924f2-162">Za Azure Active Directory zdravstveni sistem, potvrdite status **bezbednosti + usluge identiteta** navedenih na [stranici Azure status](https://azure.microsoft.com/status/).</span><span class="sxs-lookup"><span data-stu-id="924f2-162">For Azure Active Directory service health, check the status of **Security + Identity** services listed in the [Azure status page](https://azure.microsoft.com/status/).</span></span>
- <span data-ttu-id="924f2-163">Za Office usluge koje doprinose programu Microsoft Graph, potvrdite status usluga navedenim na [kontrolnoj tabli usluge Office usluga](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="924f2-163">For Office services that contribute to Microsoft Graph, check the status of services listed in the [Office Service Health Dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>
