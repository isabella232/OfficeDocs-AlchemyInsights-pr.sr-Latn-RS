---
title: Dodavanje poddomna
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "7"
- "13902"
ms.openlocfilehash: ea39984a54a15ae6167363eb5855943c8ab1120d
ms.sourcegitcommit: a097d1f8915a31ed8460b5b68dccc8d87e563cc0
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/22/2021
ms.locfileid: "59506772"
---
# <a name="adding-a-sub-domain"></a>Dodavanje poddomna

Poddomeni se mogu dodati u isti ili neki drugi zakupc od nadređenog domena. U oba slučaja morate da upravljate sopstvenim DNS postavkama na veb lokaciji registra. Ako ste dozvolili korporaciji Microsoft da upravlja vašim DNS postavkama uz NS zapise ili ako ste kupili domen od korporacije Microsoft, ne možete da dodate poddomeni ako prvo ne promenite ovo.

Prvo dodajte nadređeni domen, a zatim dodajte poddomen. Ako je poddomen u istom zakupca, nije potrebna dodatna verifikacija. Ako dodate poddomen za odvojeni zakupca, DNS txt zapis je neophodan za verifikaciju vlasništva pre dodavanja domena i dodatnih DNS zapisa za izabrane usluge.

- Da biste dodali domen ili poddomen, pratite čarobnjak za dodavanje domena [ili](https://admin.microsoft.com/Adminportal#/Domains/Wizard)ručno dodajte domen ili poddomen tako što ćete ići na podešavanje domena   >    >  **Dodaj domen.**

Ako je potrebno:

- Da biste promenili ko upravlja DNS postavkama za postojeći domen, idite na Postavke Domeni , potvrdite izbor u polju za potvrdu pored domena, a zatim izaberite stavku Upravljanje  >  [](https://admin.microsoft.com/Adminportal/Home#/Domains) **DNS-om**. U čarobnjaku izaberite **stavku Dodajte svoje DNS zapise i** dovršite čarobnjak.
- Da biste dodali poddomene na microsoft kupljen domen, prvo prenesete domen u drugi registar, a zatim napravite izmenu iznad da biste upravljali sopstvenim DNS zapisima. Uputstva možete da vidite [u članku Prenos domena od korporacije Microsoft na drugi host.](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/transfer-a-domain-from-microsoft-to-another-host)
- Ako dobijete grešku da drugi članovi ili osobe iz organizacije već koriste vaš domen, prvo ćete morati da preuzmete taj nekonvencijani nalog pre korišćenja domena. Uputstva možete da [vidite u Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/enterprise-users/domains-admin-takeover)
