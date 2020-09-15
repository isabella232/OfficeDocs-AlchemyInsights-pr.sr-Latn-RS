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
ms.openlocfilehash: 03cfd2c576cb03cbefd524a4ab6f04e2ef1eebec
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663527"
---
# <a name="add-external-users-to-a-distribution-group"></a>Dodavanje spoljnih korisnika u grupu za distribuciju

Dodavanje spoljnog kontakta u grupu za distribuciju (DG) je proces sa dva koraka:
  
1. Kreirajte kontakt e-pošte za spoljnog korisnika:
    
    1. U centru administracije idite na stranicu **Korisnici**  >  [Kontakti](https://admin.microsoft.com/adminportal/home#/Contact) . 
    
    2. Izaberite stavku **Dodaj kontakt**.
    
    3. Otkucajte informacije za kontakt i izaberite stavku **Dodaj**.
    
2. Dodajte kontakt e-pošte u svoj DG:
    
    1. U centru administracije idite na stranicu grupe **grupa**  >  [Groups](https://admin.microsoft.com/adminportal/home#/groups) . 
    
    2. Pronađite generalnog direktora kom želite da dodate spoljnog korisnika i izaberite ga da biste otvorili dijalog uređivanje.
    
    3. Na kartici **članovi** izaberite stavku **Prikaži sve članove**. 
    
    4. Izaberite stavku **Dodaj članove**.
    
    5. Izaberite kontakt koji ste kreirali na prethodnom koracima, a zatim izaberite stavku **Sačuvaj**.
    
Ako nakon praćenja ovih koraka spoljni korisnici ne mogu da šalju e-poruke na DG ili ne primaju e-poruke iz nje, možda je DG označen tako da omogući e-poruke samo od unutrašnjih korisnika. Možete da potvrdite ovu konfiguraciju i da je popravite posle uputstva [ovde](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).
  
 **Napomena:** Ova uputstva se ne primenjuju ako je tip grupe "Microsoft 365 Group" umesto "grupa za distribuciju". Ako je to slučaj, možete da dodate spoljnog korisnika direktno u grupu iz programa Outlook. Detaljne informacije o Microsoft 365 grupama gosti, kao i uputstva za dodavanje spoljnih gostiju mogu se pronaći u [ovom članku](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).
  