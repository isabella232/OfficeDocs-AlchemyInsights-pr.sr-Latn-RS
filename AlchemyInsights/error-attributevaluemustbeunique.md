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
ms.openlocfilehash: 37d6764d19d9cfbb0899a5ab85a4b1530896568adc364122075b7d6f2a32970a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "54002134"
---
# <a name="error-attributevaluemustbeunique"></a>Greška: AttributeValueMustBeUnique

Najčešći razlog za AtributValueMustBeUnique grešku je da dva objekta sa različitim SourceAnchor (immutableId) imaju istu vrednost za ProxyAddresses i/ili UserPrincipalName atribute. Da biste popravili grešku AttributeValueMustBeUnique:
  
1. Identifikujte dupliranu vrednost proxyAddresses, userPrincipalName ili drugu vrednost atributa koja izaziva grešku. Takođe identifikujte koji su dva (ili više) objekata uključena u neusaglašenost. Izveštaj koji je generisao Azure AD Povezivanje Health for sync može da vam pomogne da identifikujete dva objekta.
    
2. Identifikujte objekat koji bi trebalo da nastavi da ima dupliranu vrednost, a koji objekat ne bi trebalo.
    
3. Uklonite dupliranu vrednost iz objekta koji NE bi trebalo da ima tu vrednost. Imajte napom da treba da promenite direktorijum u kojem je objekat iz izvora. U nekim slučajevima ćete možda morati da izbrišete jedan od objekata koji su neusaglašeni.
    
4. Ako ste promenili Povezivanje AD, dozvolite da Azure AD Povezivanje sinhronizuje promenu kako bi se greška ispravila.
    

