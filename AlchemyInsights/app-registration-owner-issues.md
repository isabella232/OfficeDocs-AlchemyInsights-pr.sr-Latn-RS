---
title: Problemi vlasnika registracije aplikacije
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
- "9004352"
- "9655"
ms.openlocfilehash: cd7533f09ed8361e134b81979532cdebbf49971c54553a0172c7527f30e319bb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "53951147"
---
# <a name="app-registration-owner-issues"></a>Problemi vlasnika registracije aplikacije

Ovo su dostupni metodi za dodavanje principala kao vlasnika za registracije aplikacija:

- Korišćenje modula Azure AD PowerShell –

    `Connect-AzureAd`

    `Add-AzureADApplicationOwner -ObjectId <Application ObjectId>-RefObjectId <ObjectID of principal to assign as owner>`

    Referenca: [Add-AzureADApplicationOwner (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/add-azureadapplicationowner)
- Korišćenje Azure CLI - `az ad app owner add`

    Referenca: [vlasnik aplikacije az ad](https://docs.microsoft.com/cli/azure/ad/app/owner)
- Korišćenje MS Graph -

    Referenca: [Dodavanje vlasnika – Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-post-owners)
- Korišćenje Azure AD portala – možete da se portal.azure.com [>](https://portal.azure.com/) Azure Active Directory > Registracija aplikacija > Izaberite aplikaciju > Vlasnici > Dodaj vlasnike

**Ne možete da prikažete aplikaciju na bleju registracija aplikacije, čak i ako ste vlasnik te aplikacije?**

Vlasnik aplikacije nije administrativna uloga. Ako je omogućena postavka Ograniči pristup [Azure AD portalu](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions) za administraciju, samo će administracija moći da prikaže aplikacije na portalu za registraciju aplikacija. Da bi vlasnik mogao da prikaže aplikacije, onemogući ovu postavku (Postavite ovu postavku na NE) ili dodelite ulogu vlasnika samo za određenu aplikaciju. Međutim, biće vam potrebna licenca za Azure AD Premium P2 i [omogućite](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure)Privileged Identity Management.
