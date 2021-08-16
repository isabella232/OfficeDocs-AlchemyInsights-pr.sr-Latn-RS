---
title: Brisanje ili vraćanje aplikacija u prethodno stanje
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
- "9004335"
- "7737"
ms.openlocfilehash: 0c7be98650ca87f36b66f0bb38fb665fc81525b7f3410da14b99fb67468c1e73
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "54102585"
---
# <a name="delete-or-restore-applications"></a>Brisanje ili vraćanje aplikacija u prethodno stanje

**Da biste izbrisali aplikaciju iz Azure AD zakupca:**

1. Na **Azure AD portalu izaberite** **stavku Enterprise aplikacije**. Zatim pronađite i izaberite aplikaciju koju želite da izbrišete.
2. U **odeljku Upravljanje** u levom oknu izaberite stavku **Svojstva.**
3. Izaberite **stavku** Izbriši , a **zatim izaberite** Da da biste potvrdili da želite da izbrišete aplikaciju iz Azure AD zakupca.

Više informacija o tome kako da izbrišete aplikaciju potražite u brzom startu: Brisanje aplikacije iz [Azure Active Directory (Azure AD) zakupca.](https://docs.microsoft.com/azure/active-directory/manage-apps/delete-application-portal#delete-an-application-from-your-azure-ad-tenant)

U programu PowerShell, cmdlet [Remove-AzureApplicationProxyApplication](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplicationproxyapplication) uklanja konfiguracije proxy servera aplikacije iz određene aplikacije u programu Azure Active Directory i može potpuno da izbriše aplikaciju ako je navedena.

Izbrisanu **aplikaciju možete da vratite u prethodno stanje** pomoću programa PowerShell. Kada identifikovana aplikacija koje želite da vratite u prethodno stanje, možete da je vratite u prethodno stanje [koristeći Restore-AzureADDeletedApplication](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication).
