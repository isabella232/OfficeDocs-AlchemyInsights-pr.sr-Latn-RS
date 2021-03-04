---
title: Problem sa jednim korisnikom
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
- "9004687"
- "8469"
ms.openlocfilehash: f3564063a3adf291ec4909ffeb2f6de0e478da96
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/04/2021
ms.locfileid: "50430205"
---
# <a name="problem-with-single-user"></a>Problem sa jednim korisnikom

- Korisnik možda nije dodeljen zato što usluga još uvek nije imala priliku da proceni korisnika. Pregledajte smernice za koliko traje obezbeđivanje, kao i traka toka vremena, na stranici za konfigurisanje obezbeđivanja. Ako se čvrsto stanje navedeno u odeljku dodatni detalji nalazi pre datuma kada je korisnik kreiran/ažuriran/izbrisan, to znači da još uvek nismo procenili korisnika. U ovom scenariju, najbolje je da sačekate da se završi usluga obezbeđivanje.

  - Imajte u vidu da je naša usluga samo svesna promena u korisniku u izvornom sistemu (Cloud HR). Mora da postoji važeća promena u izvornom sistemu za Azure AD da biste otkrili promenu i doišli u aktivni direktorijum.
- Polje za obezbeđivanje je procenilo korisnika i utvrđeno je da ne bi trebalo da bude dodeljen:
  - Ako ste konfigurisali filter zasnovan na atributu, uverite se da korisnik ispunjava kriterijume koje ste naveli.
  - Ako korisnici već postoje u ciljnom sistemu i stanju korisnika u odnosu na izvor i ciljnu verziju, nećemo preduzimati nikakvu dalju radnju.
- Usluga obezbeđivanja pokušava da dodeli korisnika i nije uspela. Za ove scenarije Pregledajte karticu Rešavanje problema i preporuke za evidentiranje stavki:
  - Zahtevani atribut na korisniku možda nedostaje u lokalnom programu Active Directory ili Azure AD. Na primer, korisnički Principalname ili pravila za generaciju imena ne generišu odgovarajuću vrednost.
  - Podudarni atribut (obično je zaposlenom) ne rešava jedinstvenog korisnika u lokalnom aktivnom direktorijumu ili Azure AD. Na primer, postoje dva korisnika sa istim zaposlenim ID-om u REKLAMI i usluga vraća kôd greške koji označava duplirane odredišne stavke za istu izvornu stavku.

Da biste pregledali evidentiranje za jednog korisnika i grupe, pogledajte [članak Pregledanje evidencija resursa za problem sa određenim korisnikom](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs).
