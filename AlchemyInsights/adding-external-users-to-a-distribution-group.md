---
title: Dodavanje spoljnih korisnika u grupu za distribuciju
ms.author: chrisda
author: chrisda
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: d8c06c81ecc66df0fbaa4cac9908178cdc1d9c6bdc38d19010c7b55e9bca8776
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "53934847"
---
# <a name="add-external-users-to-a-distribution-group"></a>Dodavanje spoljnih korisnika u grupu za distribuciju

Dodavanje spoljnog kontakta u grupu za distribuciju (DG) je proces od dva koraka:
  
1. Kreiranje kontakta pošte za spoljnog korisnika:
    
    1. U centru aktivnosti idite na stranicu **"Kontakti**  >  [korisnika".](https://admin.microsoft.com/adminportal/home#/Contact) 
    
    2. Izaberite **stavku Dodaj kontakt**.
    
    3. Otkucajte informacije za kontakt i izaberite stavku **Dodaj**.
    
2. Dodajte poštanski kontakt u DG:
    
    1. U centru za administaciju idite na **stranicu**  >  [Grupe.](https://admin.microsoft.com/adminportal/home#/groups) 
    
    2. Pronađite DG u koju želite da dodate spoljnog korisnika i izaberite ga da biste otvorili dijalog "Uređivanje".
    
    3. Na kartici **Članovi** izaberite stavku **Prikaži sve članove i upravljaj članovima**. 
    
    4. Izaberite **stavku Dodaj članove**.
    
    5. Izaberite kontakt pošte koji ste kreirali u prethodnom koraku, a zatim izaberite **stavku Sačuvaj**.
    
Ako posle sledećih koraka vaši spoljni korisnici ne mogu da šalju e-poruke u DG ili ne primaju e-poruke iz DG, moguće je da je DG označen da dozvoljava samo e-poruke od internih korisnika. Ovu konfiguraciju možete da proverite i popravite ako sledite uputstva [ovde.](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online)
  
 **Napomogućeno:** Ova uputstva se ne primenjuju ako je tip vaše grupe "grupa Microsoft 365" umesto "Grupa za distribuciju". Ako je to slučaj, spoljnog korisnika možete dodati direktno u grupu iz Outlook. Detaljne informacije o gostima Microsoft 365 Grupe, kao i uputstva za dodavanje spoljnih gostiju možete pronaći u ovom [članku.](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx)
  