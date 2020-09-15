---
title: Greška u Pripisanju
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
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: 4627a7ae34b0dd9f16538ef75ac8792672dcc056
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47709165"
---
# <a name="error-attributevaluemustbeunique"></a>Greška: Autortivaluemustbeunikatna

Najčešći razlog za Pripisanjakebrnejedinstvenoj grešci su dva objekta sa različitim vrednostima Sourcesfunkcija (Imunotabenid) imaju istu vrednost za atribute Proklacija i/ili UserPrincipalName. Da biste popravili grešku "Pripisavanje vrednosti"
  
1. Identifikujte duplirane Proxyadrese, userPrincipalName ili drugi atribut atributa koji uzrokuje grešku. Takođe identifikuju dva (ili više) objekata koji su uključeni u neusaglašenost. Izveštaj koji generiše Azure AD Connect zdravstvo za sinhronizaciju može vam pomoći da identifikujete dva objekta.
    
2. Utvrdite koji objekat treba da nastavi da ima duplisanu vrednost i koji objekat ne bi trebalo da bude.
    
3. Uklonite duplisanu vrednost iz objekta koji ne bi trebalo da ima tu vrednost. Imajte u vidu da bi trebalo da promenite fasciklu u kojoj se nalazi objekat. U nekoliko slučajeva možda ćete morati da izbrišete jedan od objekata koji su neusaglašeni.
    
4. Ako ste izvršili promene u lokalnoj REKLAMI, neka Azure AD poveže sinhronizovanje promene za ispravnost.
    

