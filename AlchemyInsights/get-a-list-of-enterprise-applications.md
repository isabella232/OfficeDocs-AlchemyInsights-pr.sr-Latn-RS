---
title: Nabavite listu Enterprise aplikacija
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
- "9004342"
- "9837"
ms.openlocfilehash: f5c1a77e415d4bbaa5718a6668af95934db7e5ae
ms.sourcegitcommit: e5f261f95ffc6074cce89e62ef8c4e9fd519d3ee
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/26/2021
ms.locfileid: "51405514"
---
# <a name="get-a-list-of-enterprise-applications"></a><span data-ttu-id="7198b-102">Nabavite listu Enterprise aplikacija</span><span class="sxs-lookup"><span data-stu-id="7198b-102">Get a list of Enterprise Applications</span></span>

1. <span data-ttu-id="7198b-103">Da biste prikazali listu poslovnih aplikacija (sve aplikacije ili filtrirane po imenu za prikaz, **ID-u,** UR-ovima identifikatora itd.) putem Powershell komande, pogledajte [Get-AzureADApplication (AzureAD).](https://docs.microsoft.com/powershell/module/azuread/get-azureadapplication)</span><span class="sxs-lookup"><span data-stu-id="7198b-103">To **get a list of enterprise applications** (all applications or filtered by Display name, ID, Identifier URIs, etc.) through Powershell command, see [Get-AzureADApplication (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadapplication).</span></span>
2. <span data-ttu-id="7198b-104">Da biste listu glavnih objekata usluge (sve objekte ili filtrirali po ID-u) putem Powershell komande, pogledajte [Get-AzureADServicePrincipal (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadserviceprincipal).</span><span class="sxs-lookup"><span data-stu-id="7198b-104">To get a list of service principal objects (all objects or filtered by ID) through Powershell command, see [Get-AzureADServicePrincipal (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadserviceprincipal).</span></span>
3. <span data-ttu-id="7198b-105">Ako želite da dobijete listu samL konfigurisanih aplikacija, sledeće **PowerShell skripte vam** mogu pomoći:</span><span class="sxs-lookup"><span data-stu-id="7198b-105">If you want to **get a list of SAML configured apps, following PowerShell scripts** may help you:</span></span>

    <span data-ttu-id="7198b-106">Svaka aplikacija bi bila OAuth aplikacija ili SAML aplikacija (i galerija i aplikacije koje nisu u galeriji) ima dva objekta kreirana u AAD-u kada dođe do registracije.</span><span class="sxs-lookup"><span data-stu-id="7198b-106">Every Application be it an OAuth app or SAML app (both gallery and non-gallery apps) would have two objects created in AAD when their registration happens.</span></span> <span data-ttu-id="7198b-107">Jedan se naziva objekat aplikacije, a drugi je principal objekta usluge.</span><span class="sxs-lookup"><span data-stu-id="7198b-107">One is called the Application Object and the other is the Service Principal object.</span></span> <span data-ttu-id="7198b-108">Kada primenite svojstva glavnog objekta usluge pomoću programa PowerShell, primetiće se da svaka aplikacija ima određeni broj oznaka povezanih sa njim na slovima:</span><span class="sxs-lookup"><span data-stu-id="7198b-108">When you dump the properties of a Service Principal Object using PowerShell, you would find that every application has a certain number of Tags associated with it like:</span></span>

    - <span data-ttu-id="7198b-109">OAuth aplikacije će imati oznaku "**WindowsAzureActiveDireDirectoryIntegratedApp**"</span><span class="sxs-lookup"><span data-stu-id="7198b-109">OAuth apps would have a tag called "**WindowsAzureActiveDirectoryIntegratedApp**"</span></span>
    - <span data-ttu-id="7198b-110">Gallery SAML Apps would have a tag called "**WindowsAzureActiveDirectoryGalleryApplicationPrimaryV1**"</span><span class="sxs-lookup"><span data-stu-id="7198b-110">Gallery SAML Apps would have a tag called "**WindowsAzureActiveDirectoryGalleryApplicationPrimaryV1**"</span></span>
    - <span data-ttu-id="7198b-111">SamL aplikacije koje nisu u galeriji imaće oznaku **"WindowsAzureActiveDireDirectoryCustomSingleSignOnApplication**"</span><span class="sxs-lookup"><span data-stu-id="7198b-111">Non-Gallery SAML Apps would have a tag called "**WindowsAzureActiveDirectoryCustomSingleSignOnApplication**"</span></span>

    <span data-ttu-id="7198b-112">Tako možete da koristite ove oznake i otkrijete koja je to aplikacija.</span><span class="sxs-lookup"><span data-stu-id="7198b-112">Hence, you can use these tags and find out what kind of app it is.</span></span> <span data-ttu-id="7198b-113">Oznaka **"WindowsAzureActiveDireCtorectoryIntegratedApp"** je uobičajena za sve tipove aplikacija.</span><span class="sxs-lookup"><span data-stu-id="7198b-113">The tag "**WindowsAzureActiveDirectoryIntegratedApp**" is common to all types of apps.</span></span> <span data-ttu-id="7198b-114">Možete da koristite sledeći sekcijal da biste naveli sve SAML aplikacije (i galerija i ne-galerija):</span><span class="sxs-lookup"><span data-stu-id="7198b-114">You can use following snippet to list all the SAML apps (both gallery and non-gallery):</span></span>

    `$type = "SAML APP"`

    `Get-AzureADServicePrincipal -All true | Where-Object {(.Tags -contains "WindowsAzureActiveDirectoryGalleryApplicationNonPrimaryV1") -or (_.Tags -contains "WindowsAzureActiveDirectoryCustomSingleSignOnApplication")} | Select DisplayName, @{Name="AppType"; Expression={type}}_.`

    <span data-ttu-id="7198b-115">Više informacija potražite u temi Identifikovanje aplikacija omogućenih za [SAML u Azure AD.](https://docs.microsoft.com/answers/questions/24259/identify-saml-enabled-apps-in-azure-ad.html)</span><span class="sxs-lookup"><span data-stu-id="7198b-115">For more information, see [Identify SAML-enabled apps in Azure AD](https://docs.microsoft.com/answers/questions/24259/identify-saml-enabled-apps-in-azure-ad.html).</span></span>

4. <span data-ttu-id="7198b-116">**Pronađite i navedite** samo Veb aplikacije: Koristite dolenavedenu komandu da biste nabavili sve Azure AD aplikacije sa tipom aplikacije "Web app/API"</span><span class="sxs-lookup"><span data-stu-id="7198b-116">**Find and list only Web applications**: Use the below command to get all Azure AD applications with the application type "Web app/API"</span></span>

    <span data-ttu-id="7198b-117">Get-AzureADApplication -All:$true | Where-Object { $_. PublicClient -ne $true } | FT</span><span class="sxs-lookup"><span data-stu-id="7198b-117">Get-AzureADApplication -All:$true | Where-Object { $_.PublicClient -ne $true } | FT</span></span>
5. <span data-ttu-id="7198b-118">**Pronađite i navedite samo** ove prateće aplikacije: Pokrenite sledeću komandu da biste nabavili sve prateće aplikacije klijenta (desktop/mobile device).</span><span class="sxs-lookup"><span data-stu-id="7198b-118">**Find and list Native applications alone**: Run the following command to get all the native client (desktop/mobile device) applications.</span></span>

    <span data-ttu-id="7198b-119">Get-AzureADApplication -All:$true | Where-Object { $_. PublicClient -eq $true } | FT</span><span class="sxs-lookup"><span data-stu-id="7198b-119">Get-AzureADApplication -All:$true | Where-Object { $_.PublicClient -eq $true } | FT</span></span>
6. <span data-ttu-id="7198b-120">**Izvezi sve registrovane detalje Azure AD** aplikacije u CSV: Dolenavedna komanda izvozi sve Azure AD aplikacije sa neophodnim detaljima u csv datoteku:</span><span class="sxs-lookup"><span data-stu-id="7198b-120">**Export All Registered Azure AD Application Details to CSV**: The below command exports all the Azure AD apps with required details to csv file:</span></span>

    - <span data-ttu-id="7198b-121">Get-AzureADApplication -All:$true | Select-Object DisplayName, AppID, PublicClient, AvailableToOtherTenants, HomePage, LogoutUrl |</span><span class="sxs-lookup"><span data-stu-id="7198b-121">Get-AzureADApplication -All:$true | Select-Object DisplayName, AppID, PublicClient, AvailableToOtherTenants, HomePage, LogoutUrl |</span></span>
    - <span data-ttu-id="7198b-122">Export-Csv "C:\AzureADApps.csv" -NoTypeInformation -Encoding UTF8</span><span class="sxs-lookup"><span data-stu-id="7198b-122">Export-Csv "C:\AzureADApps.csv" -NoTypeInformation -Encoding UTF8</span></span>

7. <span data-ttu-id="7198b-123">**Potrebno je da izvezete listu nekorišćenih Azure aplikacija** – izveštaj nadzora</span><span class="sxs-lookup"><span data-stu-id="7198b-123">**Need to export a list of unused Azure apps** – Audit report</span></span>

    <span data-ttu-id="7198b-124">Azure AD može da pokazuje evidencije aplikacija samo u 30 dana ako imate Azure AD Premium licencu.</span><span class="sxs-lookup"><span data-stu-id="7198b-124">Azure AD can show application logs for only up to 30 days provided you have Azure AD Premium license.</span></span>
    <span data-ttu-id="7198b-125">Imate dve opcije da podatke zadržite duže od 30 dana.</span><span class="sxs-lookup"><span data-stu-id="7198b-125">You have two options to retain the data for longer than 30 days.</span></span> <span data-ttu-id="7198b-126">Azure [AD AI-je](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-reporting-api) možete da koristite da biste programski preuzeli podatke i uskladištili ih u bazu podataka.</span><span class="sxs-lookup"><span data-stu-id="7198b-126">You can use the [Azure AD Reporting APIs](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-reporting-api) to retrieve the data programmatically and store it in a database.</span></span> <span data-ttu-id="7198b-127">Druga mogućnost je da integrišete evidencije nadzora u SIEM sistem nezavisnog korisnika.</span><span class="sxs-lookup"><span data-stu-id="7198b-127">Alternatively, you can integrate audit logs into a third party SIEM system.</span></span>

    <span data-ttu-id="7198b-128">Možete i da preuzmete listu aplikacija za sve aplikacije i u vlasništvu aplikacija u okviru Azure Active directory>Registracije aplikacija>Preuzmi>Preuzmite sve aplikacije/u vlasništvu aplikacija.</span><span class="sxs-lookup"><span data-stu-id="7198b-128">You can also download the app list for all applications and owned applications under Azure Active directory>App Registrations>Download>All applications/Owned applications.</span></span>

    <span data-ttu-id="7198b-129">Da biste videli listu aplikacija putem usluge MS Graph, pogledajte Članak Aplikacije liste [– Microsoft Graph v1.0 i](https://docs.microsoft.com/graph/api/application-list) tip resursa aplikacije – Microsoft [Graph v1.0.](https://docs.microsoft.com/graph/api/resources/application)</span><span class="sxs-lookup"><span data-stu-id="7198b-129">To get a list of applications through MS Graph, see [List applications - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-list) and [application resource type - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/resources/application).</span></span>
