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
# <a name="consistencyguid--sourceanchor-behavior"></a>DoslednoGuid / sourceAnchor ponašanje

Azure AD Connect (verzija 1.1.524.0 i posle) sada olakšava korišćenje msDS-ConsistencyGuid kao atributa sourceAnchor. Kada koristite ovu funkciju, Azure AD Connect automatski konfiguriše pravila sinhronizacije na:
  
- Koristite msDS-ConsistencyGuid kao sourceAnchor atribut za objekte korisnika. ObjectGUID se koristi za druge tipove objekata.
    
- Za sve date objekte u kojima nije uklonjen atribut msDS-ConsistencyGuid, Azure AD Connect upisuje svoju objectGUID vrednost nazad u atribut msDS-ConsistencyGuid u prethodnom aktivnom direktorijumu. Kada se napiši atribut msDS-ConsistencyGuid, Azure AD Connect zatim izvozi objekat u Azure AD.
    
 **Napomogućeno:** Kada se besmisleni AD objekat uveze u Azure AD Connect (to jest, uveze u AD Connector Space i projektuje se u Metaverse), više ne možete da promenite njegovu izvornu vrednostAnchor. Da biste naveli izvorAnchor vrednost za dati objekat na lokaciji AD, konfigurišite njegov atribut msDS-ConsistencyGuid pre nego što se uveze u Azure AD Connect. 
  
Više informacija o sourceAnchor i ConsistencyGuid potražite u sledećim [temama: Azure AD Connect: Koncepti dizajna](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

