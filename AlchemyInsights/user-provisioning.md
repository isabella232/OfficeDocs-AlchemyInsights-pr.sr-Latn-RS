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
ms.openlocfilehash: 12490df735ca8c524058404df92db79c6c5682fe2ecafe2b42baed70fa3ab142
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "53971353"
---
# <a name="user-provisioning"></a>Obezbeđivanje korisnika

- Koristite mogućnost [obezbeđivanja na zahtev za](https://docs.microsoft.com/azure/active-directory/app-provisioning/provision-on-demand) obezbeđivanje korisnika i detaljnu dijagnostiku o koracima koje ste preduzeli.
- Da biste rešili probleme na koje nailazite prilikom obezbeđivanja korisnika i grupa, pogledajte vodič za rešavanje problema [Nema korisnika.](https://docs.microsoft.com/azure/active-directory/app-provisioning/application-provisioning-config-problem-no-users-provisioned)
- Ako primetite da korisnicima nije obezbeđeno obezbeđivanje, pogledajte obezbeđivanje [evidencija (pregled)](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs) u programu Azure Active Directory (AD). Potražite unose evidencije koji se tiče određenog korisnika.
- Povremeno ponovo pokrenite obezbeđivanje da biste pribavili sve propuštene korisnike u prethodnom ciklusu obezbeđivanja.
- Korisnik/grupa možda nisu obezbeđeni jer naša usluga još uvek nije imala priliku da proceni korisnika. Pregledajte uputstvo za to koliko dugo pružanje je potrebno, kao i traku toka na stranici za konfigurisanje obezbeđivanja. Ako je stanje navedeno u odeljku sa dodatnim detaljima pre datuma kada je korisnik kreiran/ažuriran/izbrisan, to znači da još uvek nismo procenili korisnika. U ovom scenariju najbolje je da sačekate da se usluga dodeljanja završi. Ako je stanje u redu dostignuto, preporučujemo da ponovo pokrenete pokretanje iz UI-ja na Azure portalu.
  - Imajte na umu da je naša usluga svesna samo promena korisnika ili grupe u izvornom sistemu (Azure Active Directory). Ako se korisnik/grupa ukloni direktno iz aplikacije (na primer, ServiceNow), ne znamo za te promene i ne vraćamo ih nazad na osnovu stanja korisnika u izvornom sistemu. U ovom scenariju najbolje je vratiti promenu direktno u ciljnoj aplikaciji.
- Naša usluga je procenila korisnika ili grupu i utvrdila da ne treba da se dodeluje:
  - Ako ste podesili obim na dodeljene korisnike i grupe, proverite da li je korisniku ili grupi dodeljena aplikacija.
  - Ako je korisniku/grupi dodeljena aplikacija, uverite se da nije dodeljena podrazumevanoj ulozi za pristup. Ovu ulogu nije moguće koristiti za dodeđivanje.
  - Ako ste podesili filter određivanja opsega na osnovu atributa, uverite se da korisnik ispunjava kriterijume koje ste naveli.
  - Ako korisnici već postoje u ciljnom sistemu i stanju korisnika u izvornom i ciljnom podudaranju, nećemo preduzeti dodatne radnje.
- Naša usluga je pokušavala da obezbede korisnika i nije uspela. Za ove scenarije, pregledajte karticu rešavanje problema i preporuka evidencija obezbeđivanja:
  - Neophodan atribut za korisnika može da nedostaje u Azure Active Directory ili se ne podudara sa formatom koji zahteva aplikacija nezavisnog strana. Na primer, atribut "Zemlja" za korisnika možda je postavljen na "Sjedinjene Države" kad to treba da bude SAD.
  - Atribut je referencialni atribut koji još uvek ne postoji u ciljnoj aplikaciji. Referencialni atribut je atribut koji upućuje na drugi objekat, na primer korisnika koji je član grupe. ID korisnika bi bio u atributu člana grupe, ali može da se obradi samo ako objekat korisnika na koji upućuje već postoji.
