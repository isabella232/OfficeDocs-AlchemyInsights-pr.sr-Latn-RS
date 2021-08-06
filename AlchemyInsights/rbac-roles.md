---
title: 'Uloge RBAC '
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003230"
- "7265"
ms.openlocfilehash: 1faa9f69942d39b8d78c8f3e1316f93b52eeede6408dfabc89d0f7fe38b86fb3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "53923145"
---
# <a name="rbac-rules"></a>RBAC pravila

Ako dobijete grešku dozvole: 

- Klijent sa ID-om objekta nema ovlašćenje za izvršavanje radnje nad raspodelom **(kôd: AutorizacijaFailed)**: kada pokušate da kreirate resurs, proverite da li ste trenutno prijavljeni kod korisnika kojoj je dodeljena uloga koja ima dozvolu za pisanje za resurs u izabranom polju. Na primer, da biste upravljali virtuelnim [](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor) mašinama u grupi resursa, trebalo bi da imate ulogu saradnika virtuelne mašine u grupi resursa (ili nadređenom vremenu). Listu dozvola za svaku ugrađenu ulogu pogledajte u ugrađenim ulogama za [Azure resurse.](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support)
- Nemate dozvolu za kreiranje zahteva za podršku: kada pokušate da kreirate ili ažurirate tiket za podršku, proverite da li ste trenutno prijavljeni kod korisnika čije je uloga dodeljena microsoft.support/supportTickets/write dozvola, kao što je Saradnik sa zahtevom za podršku. [](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor)
- Više nije moguće kreirati dodele uloga **(kôd: RoleAssignmentLimitExceed)**: kada pokušate da dodelite ulogu, pokušajte da smanjite broj dodela uloga dodeljivanjem uloga grupama. Azure podržava do **2000 dodela** uloga po pretplati.

Više detalja o Ulogama Azure RBAC možete da vidite u [Azure RBAC ulogama](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support).
