---
title: Više objekata ima istu e-adresu kao identitet
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1834"
- "9000247"
ms.openlocfilehash: cc932aa7ecbd1e338c409a7a6525e2c4e673b232
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439712"
---
# <a name="multiple-objects-have-the-same-email-address-as-identity"></a>Više objekata ima istu e-adresu kao identitet

**Više objekata**

Jedan od uobičajenih razloga ove greške nije u mogućnosti da usmeri zahtev za Outlook Web Access na odgovarajući način u prisustvu više objekata koji imaju istu e-adresu kao identitet. Da biste pronašli ove objekte, pokrenite sledeće komande:

· Nabavi primaocu<email address>

· Dobijanje korisnika<email address>

· Get-korisnik <email address> -softdeleteduser

· Preuzimanje-kontakt<email address>

· Get-poštansko sanduče <email address> -publikfascikla

· Preuzimanje-poštansko sanduče <email address> -includesoftdeletedpoštansko sanduče

· Preuzimanje-poštansko sanduče <email address> -inactivemailboxonly

Da biste rešili ovaj problem, uklonite više objekata sa istim identitetom e-pošte i uverite se da postoji jedan objekat sa određenim identitetom e-pošte i da je njegov tip primaoca Userpoštansko sanduče.

**Ista adresa se koristi za poslovne i potrošačke Poštanske sandučiće**

Drugi uzrok je kada se ista adresa koristi za poslovne i potrošačke Poštanske sandučiće. U ovom slučaju, korisnik mora da promeni primarni pseudonim za potrošače dok CAFFE ne podržava ovaj scenario. Ovo je stalna greška koja ne nestane bez intervencije.

Više informacija potražite u članku [Promena e-adrese ili broja telefona za Microsoft nalog](https://support.microsoft.com/help/11545/microsoft-account-rename-your-personal-account).