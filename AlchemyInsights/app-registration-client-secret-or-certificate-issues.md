---
title: Tajna klijenta za registraciju aplikacije ili problemi sa certifikatom
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
- "9685"
ms.openlocfilehash: 990648d286ec801785201e6513b70534c3d80e3f
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/23/2021
ms.locfileid: "51405334"
---
# <a name="app-registration-client-secret-or-certificate-issues"></a><span data-ttu-id="b01f9-102">Tajna klijenta za registraciju aplikacije ili problemi sa certifikatom</span><span class="sxs-lookup"><span data-stu-id="b01f9-102">App Registration client secret or Certificate issues</span></span>

<span data-ttu-id="b01f9-103">Tajni klijent aplikacije koji je u toku?</span><span class="sxs-lookup"><span data-stu-id="b01f9-103">Application client secret expiring?</span></span>

<span data-ttu-id="b01f9-104">Bez obzira na to kako je napravljena registrovana aplikacija, bilo putem standardnog procesa registracije na portalu za registraciju aplikacija ili ako je principal usluge kreiran u zakucaku pomoću pristanka aplikacije, nova tajna klijenta mora da se kreira pre isteka trenutnog i ažurira se u povezanom kodu aplikacije.</span><span class="sxs-lookup"><span data-stu-id="b01f9-104">Regardless of how the registered application was created, whether through the standard registration process in the Apps Registration portal or if the Service Principal was created in your tenant using application consent, a new Client Secret will need to be created prior to the expiration of the current one and updated in the related application code.</span></span> <span data-ttu-id="b01f9-105">Maksimalni period važenja je 2 godine.</span><span class="sxs-lookup"><span data-stu-id="b01f9-105">The maximum validity period is 2 years.</span></span> <span data-ttu-id="b01f9-106">Kao podsetnik, tajna vrednost mora da se snimi jer više neće biti vidljiva kada napustite stranicu registracije aplikacija na portalu.</span><span class="sxs-lookup"><span data-stu-id="b01f9-106">As a reminder the secret value must be recorded as it will no longer be visible after leaving the App registrations page in the portal.</span></span> <span data-ttu-id="b01f9-107">Više informacija potražite u članku Brzi start: Registrovanje aplikacije na [platformi Microsoft identiteta](https://docs.microsoft.com/azure/active-directory/develop/quickstart-register-app) i Najbolje prakse za [platformu Microsoft identiteta.](https://docs.microsoft.com/azure/active-directory/develop/identity-platform-integration-checklist#security)</span><span class="sxs-lookup"><span data-stu-id="b01f9-107">For more information, see [Quickstart: Register an app in the Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/quickstart-register-app) and [Best practices for the Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/identity-platform-integration-checklist#security).</span></span>

<span data-ttu-id="b01f9-108">Da biste saznali više, pogledajte [članak Kreiranje Azure AD aplikacije & principal usluge na portalu – platforma Microsoft identitet.](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal)</span><span class="sxs-lookup"><span data-stu-id="b01f9-108">To learn more, see [Create an Azure AD app & service principal in the portal - Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal).</span></span>
