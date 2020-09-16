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
# <a name="consistencyguid--sourceanchor-behavior"></a>Konzistencijaguid/ponašanje polja

Azure AD Connect (verzija 1.1.524.0 i posle) sada olakšava korišćenje msDS-dosledciguid kao atributa Sourceda. Kada koristite ovu funkciju, Azure AD Connect automatski konfiguriše pravila sinhronizacije na:
  
- Koristite msDS-Konzistenguid kao atribut Sourceda za korisničke objekte. GUID se koristi za druge tipove objekata.
    
- Za bilo koju datu lokalno AD User objekat čiji atribut msDS-Sledsleduslednosti nije naseljen, Azure AD Connect piše svoju datoteku objectGUID ponovo u atribut msDS-Sledsledu aktivnom direktorijumu. Kada se daje msDS-Sledsledski atribut, Azure AD Connect zatim izvozi objekat u Azure AD.
    
 **Napomena:** Kada se objekat lokalnog OGLAŠAVANJA uveze u polje Azure AD Connect (koji se nalazi, uvozi se u prostor za AD Connector i projektovan u Meaverse), više ne možete da promenite njenu vrednost Sourcepridra. Da biste naveli vrednost Sourcesads za navedeni lokalni objekat oglasa, konfigurišite atribut msDS-Sledsledslednaslednosti pre nego što se uveze u Azure AD Connect. 
  
Da biste dobili više informacija o pristupačnoj boji i Slednošću Cyguid, pogledajte sledeće: [Azure AD Connect: koncepti dizajna](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

