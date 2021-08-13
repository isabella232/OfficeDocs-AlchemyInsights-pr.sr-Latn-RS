---
title: Sinhronizacija lozinki
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "8619"
ms.openlocfilehash: 3cdde086e535d2397b4d1a8a66903121a5217015ca055fb9f8d025b0842f044b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "53960849"
---
# <a name="password-synchronization"></a>Sinhronizacija lozinki

**Sinhronizacija hasha lozinki uopšte ne funkcioniše**

Neki uobičajeni problemi na koje klijenti nailaziu kada sinhronizacija hasha lozinki ne funkcioniše su:

- Nalogu Active Directory koji koristi Azure AD Povezivanje za komunikaciju sa uslugom Active Directory nije dodeljena dozvola **Replicate Directory Changes** and **Replicate Directory Changes All** permissions, koje su neophodne za sinhronizaciju lozinki – Ovo morate da rešite tako što ćete dodeliti ove dozvole Active Directory nalogu.
- Sinhronizacija hasha lozinki je onemogućena kada administrator  promeni metod "Korisnik Sign-In" iz Sinhronizacije lozinki u drugu opciju kao što je Povezivanje sa **AD FS-om** u čarobnjaku Azure AD Povezivanje – Ovo možete da rešite tako što ćete ponovo omogućiti funkciju sinhronizacije **hasha** lozinki u čarobnjaku za Azure AD Povezivanje.
- Problem sa povezivanjem sa društvenim mrežama Active Directory. Na primer, neki kontroleri domena ne mogu da pristupe uslugi Azure AD Povezivanje ili zaštitni zid blokira [portove](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-ports) koji su neophodni – Ovo morate da rešite tako što ćete se osigurati da povezivanje između Azure AD Povezivanje servera i povezanog objekta ispravno funkcioniše.
- Azure AD Povezivanje server je trenutno u režimu stiranja, što će dovesti do toga da server ne može da pristupi hashovima lozinki – Da biste rešili problem, pratite korake opisane u odeljku Rešavanje problema sa sinhronizacijom lozinke uz [Azure AD Povezivanje](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)sinhronizaciju – Lozinke se ne sinhronizuju.

**Sinhronizacija hasha lozinki ne funkcioniše kod nekih mojih korisnika**

1. Ako ste primetili da se hash lozinke  ne sinhronizuje za korisnika, koristite zadatak rešavanja problema u Azure AD Povezivanje da biste istražili i rešili problem. Izvršite sledeće zadatke:

    a. [Pokretanje zadatka za rešavanje problema u čarobnjaku](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-objectsync)

    b. [Koristite cmdlet alatku za rešavanje problema da biste istražili problem sinhronizacije hasha lozinki za određenu upotrebu](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)

2. Objekat active Directory korisnika je omogućen za korisnika da bi korisnik promenio lozinku pri sledećoj opciji **prijavljivanja.** Kada je ova opcija omogućena, korisniku se dodeljuje privremena lozinka i prilikom sledećeg prijavljivanja će biti zatraženo da promeni lozinku. Azure AD Povezivanje ne sinhronizuje privremene lozinke sa Azure AD.

Da biste rešili gorenavedeni problem, izvršite jedan od sledećih zadataka:

- Tražite od korisnika da se prijavi u aplikaciju (na primer, Windows računar) i promeni lozinku. Nova lozinka će se sinhronizovati sa Azure AD.
- Administrator će ažurirati lozinku korisnika bez omogućavanja opcije Korisnik mora da promeni lozinku pri sledećem prijavljivanju **i** da podeli novu lozinku sa korisnikom.

3. Objekat active Directory korisnika nije  ispravno konfigurisan za sinhronizaciju objekata ili sinhronizaciju lozinki. Da biste rešili ovaj problem, pratite korake opisane u članku Rešavanje problema sa sinhronizacijom hasha lozinke sa [Azure AD Povezivanje sinhronizacijom.](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)







