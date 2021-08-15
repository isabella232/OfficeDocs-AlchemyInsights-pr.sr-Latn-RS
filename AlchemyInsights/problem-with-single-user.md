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
ms.openlocfilehash: 8d8821cda94b2af244fa317707421f9d197b6052fb316789cd286ea8b4adf19e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "53960165"
---
# <a name="problem-with-single-user"></a>Problem sa jednim korisnikom

- Korisnik možda nije obezbeđen jer usluga još uvek nije imala priliku da proceni korisnika. Pregledajte uputstvo za to koliko dugo pružanje je potrebno, kao i traku toka na stranici za konfigurisanje obezbeđivanja. Ako je stanje navedeno u odeljku sa dodatnim detaljima pre datuma kada je korisnik kreiran/ažuriran/izbrisan, to znači da još uvek nismo procenili korisnika. U ovom scenariju najbolje je da sačekate da se usluga dodeljanja završi.

  - Imajte na umu da je naša usluga svesna samo promena korisnika u izvornom sistemu (Cloud HR). U izvornom sistemu za Azure AD mora da postoji važeća promena da bi Azure AD otkrio promenu i preneo je u Active Directory.
- Usluga dodeljanja je procenila korisnika i utvrdila da ne treba da se dodeluje:
  - Ako ste podesili filter određivanja opsega na osnovu atributa, uverite se da korisnik ispunjava kriterijume koje ste naveli.
  - Ako korisnici već postoje u ciljnom sistemu i stanju korisnika u izvornom i ciljnom podudaranju, nećemo preduzeti dodatne radnje.
- Usluga obezbeđivanja je pokušavala da obezbede korisnika i nije uspela. Za ove scenarije, pregledajte karticu rešavanje problema i preporuka evidencija obezbeđivanja:
  - Neophodan atribut za korisnika može da nedostaje u programu Active Directory ili Azure AD. Na primer, userPrincipalName ili sAMAccountName pravila generacije ne generišu pravu vrednost.
  - Podudatni atribut (obično iD zaposlenog) ne razrešava se za jedinstvenog korisnika u mešovitoj kompaniji Active Directory ili Azure AD. Na primer, postoje dva korisnika sa istim ID-om zaposlenog u AD i usluga vraća kôd greške koji ukazuje na duplirane ciljne stavke za istu izvornu stavku.

Da biste pregledali evidencije za pojedinačnog korisnika i grupe, pogledajte pregled evidencija [dodeljivanja za problem sa određenim korisnikom.](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-provisioning-logs)
