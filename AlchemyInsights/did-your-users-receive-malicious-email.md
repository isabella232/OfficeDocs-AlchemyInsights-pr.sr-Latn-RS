---
title: Da li su korisnici dobili zlonamernu e-poštu
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002907"
- "5594"
- "3100017"
- "2578"
ms.openlocfilehash: 525af0b29ffa291ddf69f6f2d97f505e93342989
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/13/2021
ms.locfileid: "58326720"
---
# <a name="did-your-users-receive-malicious-email"></a>Da li su korisnici dobili zlonamernu e-poštu?

Sada možete prijaviti zlonamernu e-poštu korporaciji Microsoft [pomoću prosleđivanja na Microsoft 365 zaštitnik portalu.](https://sip.security.microsoft.com/reportsubmission?viewid=admin)

Poruke koje se prosleđuju [u](https://security.microsoft.com/reportsubmission?viewid=admin) prosleđivanju zaduženja se skeniraju i sledeći rezultati prikazani u iskačenom prikazu detalja:

- Ako je došlo do greške prilikom potvrde identiteta e-poruke pošiljaoca u vreme isporuke.
- Informacije o broju pogodaka smernica koji su možda uticali na odluku o poruci ili su je zamenili.
- Trenutni rezultati neutralizacije koje treba videti ako su URL adrese ili datoteke sadržane u poruci bile zlonamerne ili ne.
- Povratne informacije od ocenjivača

Ako je pronađena zamena, ponovno skeniranje treba da se dovrši za nekoliko minuta. Ako nije bilo problema u potvrdi identiteta e-pošte ili ako zamena nije uticala na isporuku, onda povratne informacije od ocenjivača mogu potrajati i do jedan dan.

Ako se ne složite sa konačnom odlukom o poruci, URL adresi ili datoteci (blokirano ili neblokirano), prosledite poruku za ponovno skeniranje nakon jednog dana. Velike su šanse da odluka neće biti promenjena nakon ponovnog prosleđivanja poruke.

U međuvremenu zlonamernu e-poruku možete da uklonite iz prijemnog sandučeta korisnika tako što ćete pratiti uputstvo iz [ovog članka](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization).

- Klijenti sa uslugom Microsoft zaštitnik za Office 365 mogu da:
  - Korišćenje programa [Threat Explorer za pronalaženje i brisanje sumnjive e-pošte](https://docs.microsoft.com/microsoft-365/security/office-365-security/investigate-malicious-email-that-was-delivered)
  - [Korišćenje Sef Links za blokiranje pristupa](https://docs.microsoft.com/microsoft-365/security/office-365-security/safe-links) zlonamernom URL-u
  - Pratite korisnike koji su kliknuli na zlonamerne URL adrese i pristupili im: Prikažite [phishing URL](https://docs.microsoft.com/microsoft-365/security/office-365-security/threat-explorer)adresu i kliknite na verdim podacima  &  [Get-UrlTrace](https://docs.microsoft.com/powershell/module/exchange/get-urltrace)
  - Ručno pokretanje [automatizovanog istraživanja](https://docs.microsoft.com/microsoft-365/security/office-365-security/automated-investigation-response-office)

Takođe možete da se zaštitite od zlonamernih datoteka i URL adresa tako što ćete pratiti uputstvo u članku [Zaštita od zlonamernih URL adresa i datoteka](https://docs.microsoft.com/microsoft-365/security/office-365-security/protect-against-threats).
