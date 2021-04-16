---
title: Error AttributeValueMustBeUnique
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
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: 35eb88624a5535e136ac1d01faf8e905bf00eb45
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813774"
---
# <a name="error-attributevaluemustbeunique"></a>Greška: AttributeValueMustBeUnique

Najčešći razlog za AtributValueMustBeUnique grešku je da dva objekta sa različitim SourceAnchor (immutableId) imaju istu vrednost za ProxyAddresses i/ili UserPrincipalName atribute. Da biste popravili grešku AttributeValueMustBeUnique:
  
1. Identifikujte dupliranu vrednost proxyAddresses, userPrincipalName ili drugu vrednost atributa koja izaziva grešku. Takođe identifikujte koji su dva (ili više) objekata uključena u neusaglašenost. Izveštaj koji je generisao Azure AD Connect Health za sinhronizaciju može da vam pomogne da identifikujete dva objekta.
    
2. Identifikujte objekat koji bi trebalo da nastavi da ima dupliranu vrednost, a koji objekat ne bi trebalo.
    
3. Uklonite dupliranu vrednost iz objekta koji NE bi trebalo da ima tu vrednost. Imajte napom da treba da promenite direktorijum u kojem je objekat iz izvora. U nekim slučajevima ćete možda morati da izbrišete jedan od objekata koji su neusaglašeni.
    
4. Ako ste promenili objekat na sajtu AD, dozvolite da Azure AD Connect sinhronizuje promenu kako bi greška bila popravljena.
    

