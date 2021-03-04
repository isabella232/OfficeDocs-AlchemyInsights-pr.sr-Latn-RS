---
title: GPO primena
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004400"
- "8602"
ms.openlocfilehash: d31f77e70e8456a4076a8146025f1f8ada977a06
ms.sourcegitcommit: 969219d6dff18d86d679d4d8741d1e39e4ce9539
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/03/2021
ms.locfileid: "50427561"
---
# <a name="gpo-deployment"></a>GPO primena

Postavke za korisničke i kompjuterske objekte u uslugama usluge Azure Active Directory (Azure AD DS) se često upravljaju korišćenjem objekata smernica grupe (GPOs). Azure reklame uključuju ugrađene GPOs za korisnike AADDC korisnika i AADDC kompjutere. Ove ugrađene GPOs možete prilagoditi da biste podesili smernice grupe po potrebi za okruženje. Članovi grupe Azure AD DC Administratori imaju privilegije administracije grupnih smernica u domenu Azure AD DS i mogu da kreiraju prilagođene GPOs i organizacione jedinice (use). Više informacija o tome koje su smernice grupe i kako ona funkcioniše potražite u članku [Pregled smernica grupe](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11)).

U hibridnim okruženju, smernice grupe podešene u lokalnom programu za okruženje nisu sinhronizovane sa uslugom Azure ADS. Da biste definisali postavke konfiguracije za korisnike ili računare u usluzi Azure ADS, uredite jedan od podrazumevanih GPOs ili Kreirajte prilagođeni GPO.

Ovaj članak [upravlja smernicama grupe](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) pokazuje kako da instalirate alatke za upravljanje smernicama grupe, kako ton uređuje ugrađene GPOs i kako da kreirate prilagođene GPOs.
