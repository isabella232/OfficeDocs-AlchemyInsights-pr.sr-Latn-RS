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
ms.openlocfilehash: 9b5765ff3c59b1312bead41a45a53478a96260df0567f006ab93c3ccfaf4be64
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "54044354"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>DoslednoGuid / sourceAnchor ponašanje

Azure AD Povezivanje (verzija 1.1.524.0 i novije verzije) sada olakšava korišćenje msDS-ConsistencyGuid kao atributa sourceAnchor. Kada koristite ovu funkciju, Azure AD Povezivanje automatski konfiguriše pravila sinhronizacije na:
  
- Koristite msDS-ConsistencyGuid kao sourceAnchor atribut za objekte korisnika. ObjectGUID se koristi za druge tipove objekata.
    
- Za sve date objekte u kojima nije uklonjen atribut msDS-ConsistencyGuid, Azure AD Povezivanje upisuje svoju objectGUID vrednost nazad u atribut msDS-ConsistencyGuid u prethodnom programu Active Directory. Kada se ukuca msDS-ConsistencyGuid atribut, Azure AD Povezivanje zatim izvozi objekat u Azure AD.
    
 **Napomogućeno:** Kada se besmisleni AD objekat uveze u Azure AD Povezivanje (to jest, uveze u prostor AD konektora i projektuje se u metaverznu vrednost), više ne možete da promenite njegovu izvornu vrednostUnchor. Da biste naveli izvorAnchor vrednost za dati objekat na lokaciji AD, konfigurišite njegov atribut msDS-ConsistencyGuid pre nego što se uveze u Azure AD Povezivanje. 
  
Više informacija o sourceAnchor i ConsistencyGuid potražite u sledećim [temama: Azure AD Povezivanje: Koncepti dizajna](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

