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
ms.openlocfilehash: 99e4f7e676610103355736ce847930c6c5d2d7532c4756ac4551a8d9b3020176
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "54116742"
---
# <a name="get-a-list-of-enterprise-applications"></a>Nabavite listu Enterprise aplikacija

1. Da biste prikazali listu poslovnih aplikacija (sve aplikacije ili filtrirane po imenu za prikaz, **ID-u,** UR-ovima identifikatora itd.) putem Powershell komande, pogledajte [Get-AzureADApplication (AzureAD).](https://docs.microsoft.com/powershell/module/azuread/get-azureadapplication)
2. Da biste listu glavnih objekata usluge (sve objekte ili filtrirali po ID-u) putem Powershell komande, pogledajte [Get-AzureADServicePrincipal (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadserviceprincipal).
3. Ako želite da dobijete listu samL konfigurisanih aplikacija, sledeće **PowerShell skripte vam** mogu pomoći:

    Svaka aplikacija bi bila OAuth aplikacija ili SAML aplikacija (i galerija i aplikacije koje nisu u galeriji) ima dva objekta kreirana u AAD-u kada dođe do registracije. Jedan se naziva objekat aplikacije, a drugi je principal objekta usluge. Kada primenite svojstva glavnog objekta usluge pomoću programa PowerShell, primetiće se da svaka aplikacija ima određeni broj oznaka povezanih sa njim na slovima:

    - OAuth aplikacije će imati oznaku "**WindowsAzureActiveDireDirectoryIntegratedApp**"
    - Gallery SAML Apps would have a tag called "**WindowsAzureActiveDirectoryGalleryApplicationPrimaryV1**"
    - SamL aplikacije koje nisu u galeriji imaće oznaku **"WindowsAzureActiveDireDirectoryCustomSingleSignOnApplication**"

    Tako možete da koristite ove oznake i otkrijete koja je to aplikacija. Oznaka **"WindowsAzureActiveDireCtorectoryIntegratedApp"** je uobičajena za sve tipove aplikacija. Možete da koristite sledeći sekcijal da biste naveli sve SAML aplikacije (i galerija i ne-galerija):

    `$type = "SAML APP"`

    `Get-AzureADServicePrincipal -All true | Where-Object {(.Tags -contains "WindowsAzureActiveDirectoryGalleryApplicationNonPrimaryV1") -or (_.Tags -contains "WindowsAzureActiveDirectoryCustomSingleSignOnApplication")} | Select DisplayName, @{Name="AppType"; Expression={type}}_.`

    Više informacija potražite u temi Identifikovanje aplikacija omogućenih za [SAML u Azure AD.](https://docs.microsoft.com/answers/questions/24259/identify-saml-enabled-apps-in-azure-ad.html)

4. **Pronađite i navedite** samo Veb aplikacije: Koristite dolenavedenu komandu da biste nabavili sve Azure AD aplikacije sa tipom aplikacije "Web app/API"

    Get-AzureADApplication -All:$true | Where-Object { $_. PublicClient -ne $true } | FT
5. **Pronađite i navedite samo** ove prateće aplikacije: Pokrenite sledeću komandu da biste nabavili sve prateće aplikacije klijenta (desktop/mobile device).

    Get-AzureADApplication -All:$true | Where-Object { $_. PublicClient -eq $true } | FT
6. **Izvezi sve registrovane detalje Azure AD** aplikacije u CSV: Dolenavedna komanda izvozi sve Azure AD aplikacije sa neophodnim detaljima u csv datoteku:

    - Get-AzureADApplication -All:$true | Select-Object DisplayName, AppID, PublicClient, AvailableToOtherTenants, HomePage, LogoutUrl |
    - Export-Csv "C:\AzureADApps.csv" -NoTypeInformation -Encoding UTF8

7. **Potrebno je da izvezete listu nekorišćenih Azure aplikacija** – izveštaj nadzora

    Azure AD može da pokazuje evidencije aplikacija samo u 30 dana ako imate Azure AD Premium licencu.
    Imate dve opcije da podatke zadržite duže od 30 dana. Azure [AD AI-je](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-reporting-api) možete da koristite da biste programski preuzeli podatke i uskladištili ih u bazu podataka. Druga mogućnost je da integrišete evidencije nadzora u SIEM sistem nezavisnog korisnika.

    Možete i da preuzmete listu aplikacija za sve aplikacije i u vlasništvu aplikacija u okviru Azure Active directory>Registracije aplikacija>Preuzmi>Preuzmite sve aplikacije/u vlasništvu aplikacija.

    Da biste videli listu aplikacija putem MS Graph, pogledajte Članak Aplikacije liste [– Microsoft Graph v1.0 i](https://docs.microsoft.com/graph/api/application-list) tip resursa aplikacije – Microsoft Graph [v1.0.](https://docs.microsoft.com/graph/api/resources/application)
