---
title: Skup replike
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
ms.openlocfilehash: 45cf530c3258fa3c7008c3e8251fdb7b74be6911d0487f58c5ce2530e25ca282
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "54110694"
---
# <a name="replica-set"></a>Skup replike

AADDS se naziva i kontrolisani domen. To su zapravo dva upravljača domena koje pokreće i održava backend. Dva DC-a obuhvataju jedan glavni DC i jednu replikaciju DC. Rezervne kopije u AADDS (kontrolisani domen) su automatizovani proces koji upravlja Azure platforma. U slučaju problema sa upravljanim domenom, Azure podrška može da vam pomogne u vraćanju u prethodno stanje iz rezervne kopije.

Možete da kreirate svaki skup replika u virtuelnoj mreži. Svaka virtuelna mreža mora da se podesi na svaku drugu virtuelnu mrežu koja hostuje skup replikacije kontrolisanog domena. Ova konfiguracija pravi meš-mrežnu topologiju koja podržava replikaciju direktorijuma. Virtuelna mreža može da podrži više skupova replika, pod uslovom da se svaki skup replika nalazi na različitoj virtuelnoj podmreži.

Više detalja o skupu replika možete da pročitate [u temi Koncepti skupova replika](https://docs.microsoft.com/azure/active-directory-domain-services/concepts-replica-sets).
