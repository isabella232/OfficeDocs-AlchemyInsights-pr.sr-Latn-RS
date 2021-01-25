---
title: Mapiranje atributa dodeljivanja korisnika
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/22/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7851"
- "9004348"
ms.openlocfilehash: 8bbf554c533d960a304901d7cbb492b87e9bec71
ms.sourcegitcommit: 953a8567ebcd9835f8c5c49472b223107c92549b
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 01/22/2021
ms.locfileid: "49949894"
---
# <a name="user-provisioning-attribute-mapping"></a><span data-ttu-id="24e6f-102">Mapiranje atributa dodeljivanja korisnika</span><span class="sxs-lookup"><span data-stu-id="24e6f-102">User-provisioning attribute mapping</span></span>

1. <span data-ttu-id="24e6f-103">Da biste rešili poznate probleme sa mapiranjem atributa, pogledajte prikaz [atributa](https://docs.microsoft.com/azure/active-directory/app-provisioning/known-issues#attribute-mappings).</span><span class="sxs-lookup"><span data-stu-id="24e6f-103">To troubleshoot known attribute-mapping issues, see [Attribute mappings](https://docs.microsoft.com/azure/active-directory/app-provisioning/known-issues#attribute-mappings).</span></span> 
2. <span data-ttu-id="24e6f-104">Microsoft Azure Active Directory (AD) pruža podršku za obezbeđivanje korisnika za aplikacije nezavisnih proizvođača kao što su prodavaиi, G-a i drugi.</span><span class="sxs-lookup"><span data-stu-id="24e6f-104">Microsoft Azure Active Directory (AD) provides support for user provisioning to third-party SaaS applications such as Salesforce, G Suite and others.</span></span> <span data-ttu-id="24e6f-105">Ako omogućite korisničku obezbeđivanje za aplikaciju Sahas nezavisnog proizvođača, Azure portal kontroliše svoje vrednosti atributa kroz atribute atributa.</span><span class="sxs-lookup"><span data-stu-id="24e6f-105">If you enable user provisioning for a third-party SaaS application, the Azure portal controls its attribute values through attribute-mappings.</span></span> <span data-ttu-id="24e6f-106">Da biste saznali kako da prilagodite podrazumevane atribute atributa, pogledajte članak [Prilagođavanje ugrađavanja atributa za korisnike u usluzi Azure Active Directory](https://docs.microsoft.com/azure/active-directory/app-provisioning/customize-application-attributes).</span><span class="sxs-lookup"><span data-stu-id="24e6f-106">To learn how to customize the default attribute-mappings, see [Customize user provisioning attribute-mappings for SaaS applications in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/app-provisioning/customize-application-attributes).</span></span>
    - <span data-ttu-id="24e6f-107">Da biste saznali više o snabdevanju korisničkog dodatka Seas, pogledajte članak [Šta je obezbeđivanje automatizovanog korisničkog dodatka u Azure AD?](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning)</span><span class="sxs-lookup"><span data-stu-id="24e6f-107">To learn more about SaaS app user provisioning, see [What is automated SaaS app user provisioning in Azure AD?](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning)</span></span> 
3. <span data-ttu-id="24e6f-108">Kada prilagođavate atribute atributa za korisničku obezbeđivanje, možda ćete otkriti da se atribut koji želite da mapirate ne pojavljuje na listi izvornih atributa.</span><span class="sxs-lookup"><span data-stu-id="24e6f-108">When customizing attribute-mappings for user provisioning, you might find that the attribute you want to map doesn't appear in the Source attribute list.</span></span> <span data-ttu-id="24e6f-109">[Sinhronizacija atributa iz lokalnog aktivnog direktorijuma na AZURE AD za obezbeđivanje u članku aplikacije](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning-sync-attributes-for-mapping) prikazuje kako da dodate atribut koji nedostaje tako što ćete ga sinhronizovati sa lokalnog oglasa u Azure AD.</span><span class="sxs-lookup"><span data-stu-id="24e6f-109">The [Sync an attribute from your on-premises Active Directory to Azure AD for provisioning to an application](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning-sync-attributes-for-mapping) article shows you how to add the missing attribute by synchronizing it from your on-premises AD to Azure AD.</span></span>
