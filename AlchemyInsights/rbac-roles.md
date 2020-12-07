---
title: 'Uloge u RBAC-u '
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
ms.openlocfilehash: 7c4c9d1a76f395dfb2f831d555199b76c354ca57
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 12/04/2020
ms.locfileid: "49583951"
---
# <a name="rbac-rules"></a>Pravila za RBAC

Ako dobijete grešku sa dozvolom: 

- **Klijent sa ID-om objekta nema ovlaštenja da izvršava radnju iznad opsega (kôd: autorizacija nije uspelo)**: kada pokušate da kreirate resurs, uverite se da ste trenutno prijavljeni sa korisnikom koji ima dozvolu za upisivanje u resurs na izabranom opsegu. Na primer, da biste upravljali virtuelnim mašinama u grupi resursa, trebalo bi da imate ulogu [saradnika virtualnog mašinskog](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor) programa u grupi resursa (ili nadređenom opsegu). Listu dozvola za svaku ugrađenu ulogu potražite [u članku ugrađene uloge za Azure resurse](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support).
- Nemate **dozvolu da kreirate zahtev za podršku**: kada pokušate da kreirate ili ažurirate karte za podršku, uverite se da ste trenutno prijavljeni sa korisnikom kojem je dodeljena uloga koja ima Microsoft. support/support karte/pišite dozvole, kao što je [doprinos podrške](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor).
- **Ne možete da kreirate više dodeljenih uloga (kôd: Roleromentograniиenje premašivanja)**: kada pokušate da dodelite ulogu, pokušajte da smanjite broj dodeljivanja uloga tako što dodeljujete uloge grupama. Azure podržava do **2000** dodeljivanja uloga po pretplati.

Više detalja o Azure RBAC ulogama potražite u članku [AZURE rbac uloge](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support).
