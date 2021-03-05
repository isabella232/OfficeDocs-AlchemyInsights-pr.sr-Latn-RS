---
title: Problem sa atributom i skping filtriranjem
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8470"
- "9004687"
ms.openlocfilehash: 78df24c0d8a670d678e26879cf81476f1ae9b92d
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/04/2021
ms.locfileid: "50482920"
---
# <a name="problem-with-attribute-and-scoping-filter"></a>Problem sa atributom i skping filtriranjem

**Problem sa neusaglašenim UPN vrednostima**

Radni dan za obezbeđivanje korisničkog radnog dana za OGLAŠAVANJE u AD User prikazuje poruku o grešci **HybridSynchronizationActiveDirectoryUserPrincipalNameNotUnique**. Operacija nije uspela zato što UPN vrednost obezbeđena za sabiranje/modifikacija nije jedinstvena Šumska suma. Detalji greške: **CONSTRAINT_ATT_TYPE-userPrincipalName**.

Vrednost " **Userprincipalname** " koji pokušava da podesi prilikom pravljenja oglasa korisničkog naloga već postoji u DOMENU Target a.d.. To implicira da (1) korisnik već postoji i da funkcija podudaranja sa ID-om nije uspela za korisnika ili (2) pravilo generacije UPN je Generisano neusaglašenu vrednost.

Evo koraka predloga rezolucije:

Ako korisnik već postoji i kada se podudarna identifikacija identiteta nije uspela, povežite se sa radnim danom nalogom na Active Directory nalog, a zatim potvrdite izbor u polju za proveru Ako nemaju podudaranje, to je problem sa podacima koji treba da se popravi. Na primer, ako je ID zaposlenog u toku posla 001052 i u programu AD je 1052, polje za obezbeđivanje može da se poveže sa dva naloga i pokušaće da kreira korisnika koji već postoji. Rešenje u ovom slučaju je da promenite vrednost **Zaposleneid** u reklami da biste uključene glavne nule da biste je napravili 001052.
Ako izrazi koji generišu UPN ne generišu jedinstvenu vrednost, razmotrite korišćenje funkcije dedupliranje funkcija **Seledequevalue** prilikom svakog kreiranja jedinstvene vrednosti.

**Radni dan za obezbeđivanje oglašavanja korisnika ne podešava vrednost atributa Menadžera za adninalog korisnika**

Radni dan za obezbeđivanje oglasa korisnika ne postavlja vrednost atributa **Menadžera** za AD User naloge. Postoje dva moguća scenarija kada se ovo ponašanje vidi:

1. Menadžer u radnom mestu ne može da se razreši na odgovarajući korisnički nalog za AD zato što menadžer nije u opsegu.
2. U okviru **višestruki** domeni scenariji, menadžer u toku posla nije prisutan u istom domenu kao korisnik.

Isprobajte ove korake da biste rešili problem:

1. Ako ste definisali skping filtere, prvo proverite da li se menadžer nalazi u opsegu i da li ispunjava klauzulu. Ako Menadžer ne zadovoljava filter za skping, promenite filter tako da je i menadžer u okviru operacije obezbeđivanje.
2. Ako imate više oglasa, onda konektor ima poznato ograničenje nesposobnosti da rešava reference menadžera unakrsnog domena.

Za više detalja o konfigurisanju radnog vremena za automatizovano obezbeđivanje pogledajte [članak uputstvo: konfigurisanje radnog dana za automatsko obezbeđivanje korisnika](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).













