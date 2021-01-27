---
title: Brisanje ili vraćanje aplikacija
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
ms.openlocfilehash: 4df9a98644f6bc7a30f9009719c5198db591afc9
ms.sourcegitcommit: eb685eea3ab312d404d55bfd5594a5d6d68811d1
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 01/27/2021
ms.locfileid: "50015017"
---
# <a name="delete-or-restore-applications"></a>Brisanje ili vraćanje aplikacija

**Da biste izbrisali aplikaciju iz Azure oglasa**:

1. Na **Azure AD portalu** izaberite stavku **Enterprise aplikacije**. Zatim pronađite i izaberite aplikaciju koju želite da izbrišete.
2. U odeljku **Upravljanje** u levom oknu izaberite stavku **Svojstva**.
3. Izaberite stavku **Izbriši**, a zatim kliknite na dugme **da** da biste potvrdili da želite da izbrišete aplikaciju iz Azure a.d..

Više informacija o tome kako da izbrišete aplikaciju potražite u članku [brzi Start: brisanje aplikacije iz Azure Active Directory (AZURE AD) stanara](https://docs.microsoft.com/azure/active-directory/manage-apps/delete-application-portal#delete-an-application-from-your-azure-ad-tenant).

U [programskom dodatku Power-Azureadappličapplication](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplicationproxyapplication) cmdlet uklanja konfiguracije proxy servera iz određene aplikacije u usluzi Azure Active Directory i može da izbriše aplikaciju u potpunosti ako je navedena.

**Izbrisanu aplikaciju** možete da vratite pomoću programa PowerShell. Kada se identifikuje aplikacija koju želite da vratite u prethodno stanje, možete da je vratite u prethodno stanje pomoću usluge [Restore-Azureaddeldapplic.](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication)
