---
title: API dozvole i proces pristanka
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004345"
- "9200"
ms.openlocfilehash: 23fed786e7b33adf0b6c76fc71a7e69f2cfcceb7
ms.sourcegitcommit: e5f261f95ffc6074cce89e62ef8c4e9fd519d3ee
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/26/2021
ms.locfileid: "51405439"
---
# <a name="api-permissions-and-consent-process"></a><span data-ttu-id="2ae31-102">API dozvole i proces pristanka</span><span class="sxs-lookup"><span data-stu-id="2ae31-102">API Permissions and Consent Process</span></span>

<span data-ttu-id="2ae31-103">Da bi aplikacija pristupili podacima u programu Microsoft Graph, korisnik ili administrator moraju da im dodele odgovarajuće dozvole putem procesa pristanka.</span><span class="sxs-lookup"><span data-stu-id="2ae31-103">For your app to access data in Microsoft Graph, the user or administrator must grant it the correct permissions via a consent process.</span></span> <span data-ttu-id="2ae31-104">[Microsoft Graph reference za dozvole](https://docs.microsoft.com/graph/permissions-reference) navodi dozvole povezane sa svakim glavnim skupom Microsoft Graph AČI-ja.</span><span class="sxs-lookup"><span data-stu-id="2ae31-104">[Microsoft Graph permissions reference](https://docs.microsoft.com/graph/permissions-reference) lists the permissions associated with each major set of Microsoft Graph APIs.</span></span> <span data-ttu-id="2ae31-105">Takođe pruža uputstva o tome kako da koristite dozvole.</span><span class="sxs-lookup"><span data-stu-id="2ae31-105">It also provides guidance about how to use the permissions.</span></span>

<span data-ttu-id="2ae31-106">**Podešavanje ili ažuriranje principala usluge**</span><span class="sxs-lookup"><span data-stu-id="2ae31-106">**Set up or update service principal**</span></span>

- <span data-ttu-id="2ae31-107">[Kreirajte serviceprincipal](https://docs.microsoft.com/graph/api/serviceprincipal-post-serviceprincipals) – Ovaj članak vam pokazuje kako da kreirate novi servicePrincipal objekat.</span><span class="sxs-lookup"><span data-stu-id="2ae31-107">[Create serviceprincipal](https://docs.microsoft.com/graph/api/serviceprincipal-post-serviceprincipals) - This article shows you how to create a new servicePrincipal object.</span></span>
- <span data-ttu-id="2ae31-108">Na portalu kreirajte principal [usluge & Azure AD](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) – Ovaj članak vam pokazuje kako da kreirate novu Azure Active Directory (Azure AD) aplikaciju i principal usluge koja može da se koristi sa kontrolom pristupa zasnovanom na ulozi.</span><span class="sxs-lookup"><span data-stu-id="2ae31-108">[Create an Azure AD app & service principal in the portal](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) - This article shows you how to create a new Azure Active Directory (Azure AD) application and service principal that can be used with the role-based access control.</span></span>
- <span data-ttu-id="2ae31-109">Aplikacije & glavnice usluga u [usluzi Azure AD](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) – Ovaj članak opisuje registraciju, objekte aplikacije i principale usluga u usluzi Azure Active Directory: šta su, kako se koriste i kako su međusobno povezani.</span><span class="sxs-lookup"><span data-stu-id="2ae31-109">[Apps & service principals in Azure AD](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) - This article describes application registration, application objects, and service principals in Azure Active Directory: what they are, how they are used, and how they are related to each other.</span></span>

<span data-ttu-id="2ae31-110">**Dodajte ili ažurirajte registraciju aplikacije i pružite saglasnost za administarcionu aplikaciju**</span><span class="sxs-lookup"><span data-stu-id="2ae31-110">**Add or update app registration and provide admin consent**</span></span>

- <span data-ttu-id="2ae31-111">[Kreiranje registracije aplikacije](https://docs.microsoft.com/graph/api/application-post-applications) – Ovaj članak vam pokazuje kako da kreirate novi objekat aplikacije.</span><span class="sxs-lookup"><span data-stu-id="2ae31-111">[Create an app registration](https://docs.microsoft.com/graph/api/application-post-applications) - This article shows you how to create a new application object.</span></span>
- <span data-ttu-id="2ae31-112">[Ažuriranje registracije aplikacije – API dozvole](https://docs.microsoft.com/graph/api/application-update) – Ovaj članak vam pokazuje kako da ažurirate svojstva objekta aplikacije.</span><span class="sxs-lookup"><span data-stu-id="2ae31-112">[Update an app registration - API permissions](https://docs.microsoft.com/graph/api/application-update) - This article shows you how to update the properties of an application object.</span></span>
- <span data-ttu-id="2ae31-113">[Pružite saglasnost](https://docs.microsoft.com/graph/security-authorization#grant-permissions-to-an-application) za adminitre – Za saglasnost i saglasnost u principu, zahtevamo da se saglasnost izričito izričito dodeli.</span><span class="sxs-lookup"><span data-stu-id="2ae31-113">[Provide admin consent](https://docs.microsoft.com/graph/security-authorization#grant-permissions-to-an-application) - For admin consent and consent in general, we require that an admin explicitly grants consent.</span></span>
- <span data-ttu-id="2ae31-114">[RBAC (beta)](https://docs.microsoft.com/graph/api/resources/rbacapplicationmultiple) – kontejner za upravljanje ulogom za definicije uloga i dodele uloga za Microsoft 365 RBAC dobavljače koji podržavaju više principala i višestruke prognoze u dodeli jedne uloge.</span><span class="sxs-lookup"><span data-stu-id="2ae31-114">[RBAC (beta)](https://docs.microsoft.com/graph/api/resources/rbacapplicationmultiple) - Role management container for unified role definitions and role assignments for Microsoft 365 RBAC providers that support multiple principals and multiple scopes in a single role assignment.</span></span> <span data-ttu-id="2ae31-115">Ovaj tip resursa se razlikuje od *rbacApplication* resursa.</span><span class="sxs-lookup"><span data-stu-id="2ae31-115">This is different from *rbacApplication* resource type.</span></span> <span data-ttu-id="2ae31-116">Microsoft Intune je primer takvog RBAC dobavljača.</span><span class="sxs-lookup"><span data-stu-id="2ae31-116">Microsoft Intune is an example of such a RBAC provider.</span></span> <span data-ttu-id="2ae31-117">Dodela uloge u funkciji Intune može da ima niz principala i niz grupa škodova.</span><span class="sxs-lookup"><span data-stu-id="2ae31-117">A role assignment in Intune can have an array of principals and an array of scope groups.</span></span> <span data-ttu-id="2ae31-118">**To je u beta progamu, što znači da je i dalje u razvoju i ne preporučuje se za upotrebu u proizvodnji.**</span><span class="sxs-lookup"><span data-stu-id="2ae31-118">**This is in beta, meaning that it is still in development and not recommended for use in production.**</span></span>
