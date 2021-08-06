---
title: Radni dan u AD obezbeđivanje korisnika prelazi u stanje karantina
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8471"
- "9004687"
ms.openlocfilehash: 32a5d010b95b9587e121ca1526def743fd8f371b13d1d73d3578c692839edf19
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "54036506"
---
# <a name="workday-to-ad-user-provisioning-goes-into-quarantine-state"></a>Radni dan u AD obezbeđivanje korisnika prelazi u stanje karantina

**Radni dan do obezbeđivanja korisnika usluge AD prelazi u stanje karantina i nijedan korisnik se ne kreira u AD-u**

Zadatak obezbeđivanja korisnika funkcije "Radni dan za korisnike" prešao je u stanje karantina, a evidencije nadzora prikazžuju događaje neuspešnog izvoza uz poruku o grešci **Greška: OperationsError-SvcErr: Došlo je do greške u operaciji. Za uslugu direktorijuma nije konfigurisana nijedna vrhunska referenca. Usluga direktorijuma zbog toga ne može da izda preporuke za objekte izvan ove šume.** Ova greška se obično pojavljuje ako Active Directory Container OU nije ispravno podešen ili ako postoje problemi sa mapiranjem izraza koji se koristi za **nadređenoDistinguishedName.**

Proverite da li u parametru **Podrazumevani** OU za nove korisnike možete da naiđete na beleške. Uverite se da navedeni OU već postoji u vašem OD-u. Ako koristite **nadređenoIme** u mapiranju atributa, uverite se da uvek ima poznati kontejner u okviru AD domena. Proverite događaj Izvoz u evidencijama nadzora da biste videli generisanu vrednost.

Više detalja o konfigurisanju radnog dana za automatizovano dodeljanje, pogledajte Uputstvo: Konfigurisanje radnog dana za automatsko [dodeljanje korisnika.](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)

