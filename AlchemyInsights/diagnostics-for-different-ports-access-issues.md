---
title: Dijagnoza za različiti problemi sa priključkom na portove
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9035"
- "9005220"
ms.openlocfilehash: 3673067cad7ac55f3820422dc2ec09942c393149
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036810"
---
# <a name="diagnostics-for-different-ports-access-issues"></a>Dijagnoza za različiti problemi sa priključkom na portove

Da biste rešili drugačiji problem pristupa portova, obavite sledeće korake:

1. Zaustavite/o pronalaženju virtuelnog mašinskog (VR) sa portala, ponovo pokrenite Vim i testirajte ponovo. 
2. Proverite postavke mrežne mreže za VANGOVE osobe da biste utvrdili da li imate mrežne bezbednosne grupe (NSGs) blokiranjem saobraćaja. Možete da koristite i [alatku verifikovanje IP toka sistema Network posmatrače protoka](https://docs.microsoft.com/azure/network-watcher/network-watcher-ip-flow-verify-overview?WT.mc_id=Portal-Microsoft_Azure_Support) da biste proverili da li su NSGs blokirali saobraćaj, User-Defined rute (Usus) preusmeravanje saobraćaja nazad na lokalno (' podrazumevani put ' 0.0.0.0/0) ili na mrežni aparat.
Ako i dalje nailazite na probleme posle pokušaja da pokušate da uradite korake iznad, obezbedite ime za Vim i TCP port na koji pokušavate da pošaljete poštu za dalju dijagnozu.

**Preporučeni dokumenti**

[Ograničenja i preporuke za slanje odlazne e-pošte preko porta 25](https://docs.microsoft.com/azure/virtual-network/troubleshoot-outbound-smtp-connectivity)