---
title: Sinhronizacija usluge domena
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003245"
- "7922"
- "7921"
ms.openlocfilehash: b35d3a402bc08a27a818209385c5666b901fa524
ms.sourcegitcommit: 83fe2a8d060794fdf58445b469b30a3294b7a9b6
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 01/15/2021
ms.locfileid: "49885565"
---
# <a name="domain-service-synchronization"></a><span data-ttu-id="f31b5-102">Sinhronizacija usluge domena</span><span class="sxs-lookup"><span data-stu-id="f31b5-102">Domain service synchronization</span></span>

<span data-ttu-id="f31b5-103">Objekti i akreditivi u usluzi Azure Active Directory usluge (Azure AD DS) kontrolisani domen može da se kreira lokalno u domenu ili sinhronizuje iz Azure Active Directory (Azure AD) stanara.</span><span class="sxs-lookup"><span data-stu-id="f31b5-103">Objects and credentials in an Azure Active Directory Domain Services (Azure AD DS) managed domain can either be created locally within the domain, or synchronized from an Azure Active Directory (Azure AD) tenant.</span></span> <span data-ttu-id="f31b5-104">Kada prvi put primenite Azure OGLASE, automatska sinhronizacija jednosmerne mreže se konfiguriše i inicira da kopira objekte iz usluge Azure AD.</span><span class="sxs-lookup"><span data-stu-id="f31b5-104">When you first deploy Azure AD DS, an automatic one-way synchronization is configured and initiated to replicate the objects from Azure AD.</span></span> <span data-ttu-id="f31b5-105">Ova Jednosmerna sinhronizacija i dalje se pokreće u pozadini da bi se Azure AD DS kontrolisane sa svim promenama iz Azure AD.</span><span class="sxs-lookup"><span data-stu-id="f31b5-105">This one-way synchronization continues to run in the background to keep the Azure AD DS managed domain up-to-date with any changes from Azure AD.</span></span> <span data-ttu-id="f31b5-106">Sinhronizacija sa Azure AD DS-a se ne javlja na Azure AD.</span><span class="sxs-lookup"><span data-stu-id="f31b5-106">No synchronization occurs from Azure AD DS back to Azure AD.</span></span>

<span data-ttu-id="f31b5-107">Više detalja o usluzi aure Active Directory usluge domena potražite u članku [Sinhronizacija usluge Domain](https://docs.microsoft.com/azure/active-directory-domain-services/synchronization).</span><span class="sxs-lookup"><span data-stu-id="f31b5-107">For more details on Azure Active Directory domain service synchronization, see [Domain Service Synchronization](https://docs.microsoft.com/azure/active-directory-domain-services/synchronization).</span></span> 
