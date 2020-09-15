---
title: Monitoring uslovnog pristupa
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: dcb86c54-769e-4832-9f88-bc45f1e5f36c
ms.openlocfilehash: 6083fc427e3791fdb0907198b525337a0c987c4e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47702917"
---
# <a name="monitoring-conditional-access-for-exchange"></a>Monitoring uslovnog pristupa za Exchange

Korisnici koji su usmereni na uslovno pristup dobiće obaveštenje ako ne ispune zahteve za pristup vaše organizacije. Da biste rešili, preporučujemo neka od sledećih rešenja:
  
- Ako se na uređaj pretpostavlja da je upisan, savetujte korisnika da ode na aplikaciju portala preduzeća i potvrdi da se pojavljuje na portalu preduzeća. Ako nije, korisnik treba da prijavi uređaj.
    
- U Azure portalu idite na ** \> usaglašenost uređaja**. U okviru **prati** izaberite stavku **usaglašenost uređaja**. Prikažite izveštaj usaglašenosti uređaja da biste potvrdili da je uređaj korisnika označen kao usaglašeni. 
    
- U Azure portalu idite na ** \> usaglašenost uređaja**. U okviru **Upravljanje**izaberite stavku **smernice**. Na listi smernica usaglašenosti proverite da li je profil dodeljen vašem uređaju. Ako nijedan profil nije dodeljen, Intune neće moći da potvrdi status usaglašenosti uređaja. 
    
- Uredite zadatak korisnika uslovnog pristupa.
    
1. U Azure portalu idite na **Podešavanje \> uslovne \> smernice za pristup**
    
2. Izbor smernica sa liste
    
3. Izaberite stavku **korisnici i grupe**
    
4. Da biste nekome ciljali određenu politiku, dodajte ih na listu " **ukljuci** ". Da biste se uverili da je osoba **izostavljena** iz smernica, dodajte ih na listu "Isključi". 
    
Pročitajte više: [kako nadgledati uslovno pristup uređajima](https://docs.microsoft.com/intune/conditional-access-exchange-monitor)
  

