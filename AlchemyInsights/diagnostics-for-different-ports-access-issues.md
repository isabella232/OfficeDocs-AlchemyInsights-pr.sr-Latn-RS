---
title: Dijagnostika za probleme sa pristupom portovima
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
ms.openlocfilehash: 07c108d5292965d20340da039b67744d93c0a4fc61edb8115796671f2f7f1552
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "54030916"
---
# <a name="diagnostics-for-different-ports-access-issues"></a>Dijagnostika za probleme sa pristupom portovima

Da biste rešili različite probleme sa pristupom portu, izvršite sledeće korake:

1. Zaustavite virtuelnu mašinu (VM) sa portala ili ga ponovo pokrenite, a zatim ponovo testirajte. 
2. Proverite postavke mreže VM-a da biste utvrdili da li bezbednosne grupe mreže (NSG-ove) blokiraju saobraćaj. Takođe možete da koristite alatku za proveru [toka IP](https://docs.microsoft.com/azure/network-watcher/network-watcher-ip-flow-verify-overview?WT.mc_id=Portal-Microsoft_Azure_Support) adrese mrežnog toka da biste proverili da li NSG-ove blokiraju saobraćaj, User-Defined usmeravanja (UD-ove) koja preusmerava saobraćaj nazad na lokaciju ("Podrazumevano usmeravanje" 0.0.0.0/0) ili na mrežni uređaj.
Ako i dalje naići na probleme nakon što ste pokušali gorenavedene korake, navedite VM ime i TCP port na koji pokušavate da pošaljete poštu na dalju dijagnostiku.

**Preporučeni dokumenti**

[Ograničenja i preporuke za slanje odlazne e-pošte putem porta 25](https://docs.microsoft.com/azure/virtual-network/troubleshoot-outbound-smtp-connectivity)