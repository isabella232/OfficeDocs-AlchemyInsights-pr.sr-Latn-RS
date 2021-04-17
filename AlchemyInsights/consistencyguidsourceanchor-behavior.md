---
title: DoslednoGuid / sourceAnchor ponašanje
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: eafe1ec9636cddc9d73a88beb7ae3ad9f6fad660
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/15/2021
ms.locfileid: "51817006"
---
# <a name="consistencyguid--sourceanchor-behavior"></a><span data-ttu-id="02662-102">DoslednoGuid / sourceAnchor ponašanje</span><span class="sxs-lookup"><span data-stu-id="02662-102">ConsistencyGuid / sourceAnchor behavior</span></span>

<span data-ttu-id="02662-103">Azure AD Connect (verzija 1.1.524.0 i posle) sada olakšava korišćenje msDS-ConsistencyGuid kao atributa sourceAnchor.</span><span class="sxs-lookup"><span data-stu-id="02662-103">Azure AD Connect (version 1.1.524.0 and after) now facilitates the use of msDS-ConsistencyGuid as sourceAnchor attribute.</span></span> <span data-ttu-id="02662-104">Kada koristite ovu funkciju, Azure AD Connect automatski konfiguriše pravila sinhronizacije na:</span><span class="sxs-lookup"><span data-stu-id="02662-104">When using this feature, Azure AD Connect automatically configures the synchronization rules to:</span></span>
  
- <span data-ttu-id="02662-105">Koristite msDS-ConsistencyGuid kao sourceAnchor atribut za objekte korisnika.</span><span class="sxs-lookup"><span data-stu-id="02662-105">Use msDS-ConsistencyGuid as the sourceAnchor attribute for User objects.</span></span> <span data-ttu-id="02662-106">ObjectGUID se koristi za druge tipove objekata.</span><span class="sxs-lookup"><span data-stu-id="02662-106">ObjectGUID is used for other object types.</span></span>
    
- <span data-ttu-id="02662-107">Za sve date objekte u kojima nije uklonjen atribut msDS-ConsistencyGuid, Azure AD Connect upisuje svoju objectGUID vrednost nazad u atribut msDS-ConsistencyGuid u prethodnom aktivnom direktorijumu.</span><span class="sxs-lookup"><span data-stu-id="02662-107">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory.</span></span> <span data-ttu-id="02662-108">Kada se napiši atribut msDS-ConsistencyGuid, Azure AD Connect zatim izvozi objekat u Azure AD.</span><span class="sxs-lookup"><span data-stu-id="02662-108">After the msDS-ConsistencyGuid attribute is populated, Azure AD Connect then exports the object to Azure AD.</span></span>
    
 <span data-ttu-id="02662-109">**Napomogućeno:** Kada se besmisleni AD objekat uveze u Azure AD Connect (to jest, uveze u AD Connector Space i projektuje se u Metaverse), više ne možete da promenite njegovu izvornu vrednostAnchor.</span><span class="sxs-lookup"><span data-stu-id="02662-109">**Note:** Once an on-premises AD object is imported into Azure AD Connect (that is, imported into the AD Connector Space and projected into the Metaverse), you cannot change its sourceAnchor value anymore.</span></span> <span data-ttu-id="02662-110">Da biste naveli izvorAnchor vrednost za dati objekat na lokaciji AD, konfigurišite njegov atribut msDS-ConsistencyGuid pre nego što se uveze u Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="02662-110">To specify the sourceAnchor value for a given on-premises AD object, configure its msDS-ConsistencyGuid attribute before it is imported into Azure AD Connect.</span></span> 
  
<span data-ttu-id="02662-111">Više informacija o sourceAnchor i ConsistencyGuid potražite u sledećim [temama: Azure AD Connect: Koncepti dizajna](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span><span class="sxs-lookup"><span data-stu-id="02662-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span></span>
  

