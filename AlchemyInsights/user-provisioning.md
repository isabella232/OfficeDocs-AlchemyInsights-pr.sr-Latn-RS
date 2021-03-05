---
title: Obezbeđivanje korisnika
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004348"
- "8428"
ms.openlocfilehash: bd415b2d44bccf0c2b3eccb4e38452498b748b3a
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/04/2021
ms.locfileid: "50482917"
---
# <a name="user-provisioning"></a>Obezbeđivanje korisnika

- Koristite mogućnosti za [obezbeđivanje na zahtev](https://docs.microsoft.com/azure/active-directory/app-provisioning/provision-on-demand) za obezbeđivanje korisnika i nabavite detaljnu dijagnostiku za preduzete korake.
- Da biste rešili probleme na koje naiđete prilikom obezbeđivanja korisnika i grupa, pogledajte Vodič za rešavanje problema [nijedan korisnik nije dodeljen](https://docs.microsoft.com/azure/active-directory/app-provisioning/application-provisioning-config-problem-no-users-provisioned).
- Ako primetite da korisnici nisu obezbeđeni, pogledajte odeljak [evidentiranje (pregled)](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs) u usluzi Azure Active DIRECTORY (AD). Pretraga stavki evidencije koje se odnose na određenog korisnika.
- Periodično ponovo pokrenite obezbeđivanje da biste uhvatili korisnike koji su promašili u prethodnom ciklusu dodeljivanja.
- Korisnik/grupa možda nije dodeljen zato što Naša usluga još uvek nije imala priliku da proceni korisnika. Pregledajte smernice za koliko traje obezbeđivanje, kao i traka toka vremena, na stranici za konfigurisanje obezbeđivanja. Ako se čvrsto stanje navedeno u odeljku dodatni detalji nalazi pre datuma kada je korisnik kreiran/ažuriran/izbrisan, to znači da još uvek nismo procenili korisnika. U ovom scenariju, najbolje je da sačekate da se završi usluga obezbeđivanje. Ako je postignuto stabilno stanje, preporučujemo da se ponovo pokrene sa korisničkog interfejsa na Azure portalu.
  - Imajte u vidu da je naša usluga samo svesna promena u korisniku/grupi u izvornom sistemu (Azure Active Directory). Ako se korisnik/grupa ukloni direktno u aplikaciji (na primer, ServiceNow) nismo svesni tih promena i ne vraćaj je nazad na osnovu stanja korisnika u izvornom sistemu. U ovom scenariju najbolje je da ponovo vratite promene direktno u ciljnu aplikaciju.
- Naša usluga je procenila korisnika/grupu i utvrdila da ne bi trebalo da bude obezbeđena:
  - Ako ste odredili opseg za dodeljene korisnike i grupe, potvrdite izbor u polju za proveru da li je korisnik/grupa dodeljen aplikaciji.
  - Ako je korisniku/grupi dodeljena aplikacija, uverite se da im nije dodeljena podrazumevana pristupna uloga. Nije moguće koristiti ovu ulogu za obezbeđivanje.
  - Ako ste konfigurisali filter zasnovan na atributu, uverite se da korisnik ispunjava kriterijume koje ste naveli.
  - Ako korisnici već postoje u ciljnom sistemu i stanju korisnika u odnosu na izvor i ciljnu verziju, nećemo preduzimati nikakvu dalju radnju.
- Naša usluga je pokušala da odredilo korisnika i nije uspelo. Za ove scenarije Pregledajte karticu Rešavanje problema i preporuke za evidentiranje stavki:
  - Zahtevani atribut na korisniku možda nedostaje u okviru Azure Active Directory ili se ne podudara sa formatom koji zahteva treće lice. Na primer, atribut za zemlju na korisniku može biti postavljen za Sjedinjene Države kada treba da bude mi.
  - Atribut je referentni atribut koji još uvek ne postoji u ciljnoj aplikaciji. Referencijalni atribut je atribut koji upućuje na drugi objekat, na primer, korisnika koji je član grupe. Korisnički ID se nalazi u atributu grupe, ali se može obraditi samo ako korisnik objekta na koji upućuje već postoji.
