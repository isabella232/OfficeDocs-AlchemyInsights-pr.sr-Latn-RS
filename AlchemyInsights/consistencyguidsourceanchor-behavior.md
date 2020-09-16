---
title: Konzistencijaguid/ponašanje polja
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: adac469328485696d1ee1532aa3d6828af0642eb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47756297"
---
# <a name="consistencyguid--sourceanchor-behavior"></a><span data-ttu-id="7f6bb-102">Konzistencijaguid/ponašanje polja</span><span class="sxs-lookup"><span data-stu-id="7f6bb-102">ConsistencyGuid / sourceAnchor behavior</span></span>

<span data-ttu-id="7f6bb-103">Azure AD Connect (verzija 1.1.524.0 i posle) sada olakšava korišćenje msDS-dosledciguid kao atributa Sourceda.</span><span class="sxs-lookup"><span data-stu-id="7f6bb-103">Azure AD Connect (version 1.1.524.0 and after) now facilitates the use of msDS-ConsistencyGuid as sourceAnchor attribute.</span></span> <span data-ttu-id="7f6bb-104">Kada koristite ovu funkciju, Azure AD Connect automatski konfiguriše pravila sinhronizacije na:</span><span class="sxs-lookup"><span data-stu-id="7f6bb-104">When using this feature, Azure AD Connect automatically configures the synchronization rules to:</span></span>
  
- <span data-ttu-id="7f6bb-105">Koristite msDS-Konzistenguid kao atribut Sourceda za korisničke objekte.</span><span class="sxs-lookup"><span data-stu-id="7f6bb-105">Use msDS-ConsistencyGuid as the sourceAnchor attribute for User objects.</span></span> <span data-ttu-id="7f6bb-106">GUID se koristi za druge tipove objekata.</span><span class="sxs-lookup"><span data-stu-id="7f6bb-106">ObjectGUID is used for other object types.</span></span>
    
- <span data-ttu-id="7f6bb-107">Za bilo koju datu lokalno AD User objekat čiji atribut msDS-Sledsleduslednosti nije naseljen, Azure AD Connect piše svoju datoteku objectGUID ponovo u atribut msDS-Sledsledu aktivnom direktorijumu.</span><span class="sxs-lookup"><span data-stu-id="7f6bb-107">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory.</span></span> <span data-ttu-id="7f6bb-108">Kada se daje msDS-Sledsledski atribut, Azure AD Connect zatim izvozi objekat u Azure AD.</span><span class="sxs-lookup"><span data-stu-id="7f6bb-108">After the msDS-ConsistencyGuid attribute is populated, Azure AD Connect then exports the object to Azure AD.</span></span>
    
 <span data-ttu-id="7f6bb-109">**Napomena:** Kada se objekat lokalnog OGLAŠAVANJA uveze u polje Azure AD Connect (koji se nalazi, uvozi se u prostor za AD Connector i projektovan u Meaverse), više ne možete da promenite njenu vrednost Sourcepridra.</span><span class="sxs-lookup"><span data-stu-id="7f6bb-109">**Note:** Once an on-premises AD object is imported into Azure AD Connect (that is, imported into the AD Connector Space and projected into the Metaverse), you cannot change its sourceAnchor value anymore.</span></span> <span data-ttu-id="7f6bb-110">Da biste naveli vrednost Sourcesads za navedeni lokalni objekat oglasa, konfigurišite atribut msDS-Sledsledslednaslednosti pre nego što se uveze u Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="7f6bb-110">To specify the sourceAnchor value for a given on-premises AD object, configure its msDS-ConsistencyGuid attribute before it is imported into Azure AD Connect.</span></span> 
  
<span data-ttu-id="7f6bb-111">Da biste dobili više informacija o pristupačnoj boji i Slednošću Cyguid, pogledajte sledeće: [Azure AD Connect: koncepti dizajna](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span><span class="sxs-lookup"><span data-stu-id="7f6bb-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span></span>
  

