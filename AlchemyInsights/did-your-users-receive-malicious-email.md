---
title: Da li su korisnici dobili zlonamernu e-poštu
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: 2197e7f195d789193798b80cb092d8046eb6e0be
ms.sourcegitcommit: 3c708a4a349b60b59bc623c44fb78674c685f3c2
ms.translationtype: HT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 02/18/2021
ms.locfileid: "50291806"
---
# <a name="did-your-users-receive-malicious-email"></a>Da li su korisnici dobili zlonamernu e-poštu?

- Sada možete da prijavite zlonamernu e-poštu korporaciji Microsoft putem opcije [Prosleđivanja administratora u Centru za bezbednost i usaglašenost](https://sip.protection.office.com/reportsubmission).

Poruke koje su prosleđene u [prosleđivanja administratora](https://sip.protection.office.com/reportsubmission) se skeniraju a sledeći rezultati se prikazuju u iskačućem prozoru **detalja**:

- Ako je došlo do greške prilikom potvrde identiteta e-poruke pošiljaoca u vreme isporuke.
- Informacije o broju pogodaka smernica koji su možda uticali na odluku o poruci ili su je zamenili.
- Trenutni rezultati neutralizacije koje treba videti ako su URL adrese ili datoteke sadržane u poruci bile zlonamerne ili ne.
- Povratne informacije od ocenjivača

Ako je pronađena zamena, ponovno skeniranje treba da se dovrši za nekoliko minuta. Ako nije bilo problema u potvrdi identiteta e-pošte ili ako zamena nije uticala na isporuku, onda povratne informacije od ocenjivača mogu potrajati i do jedan dan.

Ako se ne složite sa konačnom odlukom o poruci, URL adresi ili datoteci (blokirano ili neblokirano), prosledite poruku za ponovno skeniranje nakon jednog dana. Velike su šanse da odluka neće biti promenjena nakon ponovnog prosleđivanja poruke.

U međuvremenu zlonamernu e-poruku možete da uklonite iz prijemnog sandučeta korisnika tako što ćete pratiti uputstvo iz [ovog članka](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization).

- Klijenti sa uslugom Microsoft zaštitnik za Office 365 mogu da:
    - koriste [Istraživač pretnji za pronalaženje i brisanje sumnjivih e-poruka](https://docs.microsoft.com/microsoft-365/security/office-365-security/investigate-malicious-email-that-was-delivered)
    - [koriste bezbedne veze za blokiranje pristupa](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-safe-links) zlonamernim URL adresama
    - prate korisnike koji su kliknuli na zlonamernu URL adresu i pristupili joj: [Prikažite URL koji sadrži phishing i kliknite na podatke o odluci](https://docs.microsoft.com/microsoft-365/security/office-365-security/threat-explorer) & [Preuzmi-praćenjeURL-a](https://docs.microsoft.com/powershell/module/exchange/get-urltrace)
    - ručno [pokrenu automatizovano ispitivanje](https://docs.microsoft.com/microsoft-365/security/office-365-security/automated-investigation-response-office)

Takođe možete da se zaštitite od zlonamernih datoteka i URL adresa tako što ćete pratiti uputstvo u članku [Zaštita od zlonamernih URL adresa i datoteka](https://docs.microsoft.com/microsoft-365/security/office-365-security/protect-against-threats).