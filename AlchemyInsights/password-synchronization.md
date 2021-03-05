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
ms.openlocfilehash: 601649f6e5212ca03df5fcc32cd1d02c133e9170
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/04/2021
ms.locfileid: "50483082"
---
# <a name="password-synchronization"></a>Sinhronizacija lozinki

**Hash sinhronizacija lozinki uopšte ne funkcioniše**

Neki uobičajeni problemi sa kojima se suočavaju klijenti kada hash sinhronizacija lozinki ne radi su:

- Korisnički nalog usluge Active Directory koji koristi Azure AD Connect za komunikaciju sa lokalnim aktivnim direktorijumom nije odobren **replikaciju promena direktorijuma** i **replicirati promene direktorijuma sve** dozvole, koje su potrebne za sinhronizaciju lozinki – potrebno je da to rešite tako što ćete ove dozvole dodeliti usluzi Active Directory.
- Sinhronizacija lozinki je onemogućiti kada je administrator promenio metod korisničkog Sign-In iz **sinhronizacije lozinki** na drugu opciju kao što je **Federacija sa AD FS** u ČAROBNJAKU "Azure AD Connect" – to možete da popravite tako što ćete ponovo omogućiti funkciju **hash sinhronizacije lozinki** u čarobnjaku "Azure a.d. za povezivanje".
- Problem sa povezivanjem sa lokalnim aktivnim direktorijumom. Na primer, neki kontrolori domena nisu pristupačni na lokaciji Azure AD Connect ili je zabranjen pristup [Portovom](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-ports) zaštitnog zida – potrebno vam je da to rešite tako što ćete osigurati da se veza između AZURE AD Connect server i lokalnog aktivnog direktorijuma ispravno rade.
- Azure AD Connect server se trenutno nalazi u režimu postavljanja, što će dovesti do toga da server ne može da gnjavi lozinke-da reši problem, da uradite korake opisane u odeljku [Rešavanje problema sa lozinkom sinhronizacija lozinki sa lokacijom AZURE AD Connect Sync – nijedna lozinka nije sinhronizovana](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).

**Sinhronizacija lozinki ne radi za neke od mojih korisnika**

1. Ako ste primetili da se hash lozinka ne sinhronizuje za korisnika, koristite zadatak **Rešavanje problema** u okviru AZURE AD povezivanje da biste istražili i rešili problem. Obavljanje sledećih zadataka:

    Neko. [Pokreće zadatak rešavanja problema u čarobnjaku](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-objectsync)

    -. [Korišćenje cmdlet problema za istraživanje problema sa hash sinhronizacijom lozinki za određenu upotrebu](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)

2. Omogućeno je da korisnik u lokalnom programu Active Directory **Promeni lozinku pri sledećoj prijavljivanju** . Kada je ova opcija omogućena, korisniku se dodeljuje privremena lozinka i biće vam zatraženo da promenite lozinku na sledećem prijavljivanju. Azure AD Connect ne sinhronizuje privremene lozinke u Azure AD.

Da biste rešili iznad problem, obavite sledeće zadatke:

- Zamolite korisnika da se prijavi u lokalnu aplikaciju (na primer, Windows Desktop) i da promeni lozinku. Nova lozinka će se sinhronizovati sa uslugom Azure AD.
- Neka administrator ažurira lozinku korisnika bez omogućavanja opcije **korisnik mora da promeni lozinku na sledećoj prijavi** i da deli novu lozinku sa korisnikom.

3. Lokalni objekat aktivnog direktorijuma **nije ispravno konfigurisan** za sinhronizaciju objekta ili sinhronizaciju lozinki. Da biste rešili ovaj problem, slijedite korake opisane u [sinhronizaciji za rešavanje problema sa lozinkama lozinki pomoću usluge Azure AD Connect Sync](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).







