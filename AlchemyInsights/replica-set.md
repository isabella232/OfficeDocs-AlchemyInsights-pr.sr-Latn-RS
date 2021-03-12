---
title: Komplet replika
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004400"
- "9004395"
- "8265"
- "9276"
ms.openlocfilehash: 3834696ff59b7e96e90a5b660a489003dfa9729c
ms.sourcegitcommit: 581c696ec108184adae9d4bc8f47cb9247131de8
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/10/2021
ms.locfileid: "50714256"
---
# <a name="replica-set"></a>Komplet replika

ASABIRANJE se takođe zove kao upravljani domen. To su zapravo dva upravljača domena koja se pokreću i održavaju u okviru pozadine. Dva funkcija DCs uključujete jedan glavni centar za centar i jednu replikaciju. Rezervna kopija u ADODAJE (kontrolisani domen) je automatizovani proces koji upravlja Azure platformom. U slučaju problema sa upravljanim domenom, Azure podrška vam može pomoći pri ponovnom uspostavljanju iz rezervne kopije.

Pravite svaku repliku skupu u virtuelnoj mreži. Svaka virtualna mreža mora da bude u okviru svake druge virtuelne mreže koja je host skupu replika kontrolisanog domena. Ova konfiguracija kreira topologiju mreže koja podržava replikaciju direktorijuma. Virtuelna mreža može da podrži više skupova replika, pod uslovom da se svaka grupa replika nalazi u drugoj virtualnoj podmreži.

Za više detalja o skupu replika pogledajte [skupove replika koncepata](https://docs.microsoft.com/azure/active-directory-domain-services/concepts-replica-sets).
