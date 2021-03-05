---
title: Radni dan za obezbeđivanje oglasa korisnika ide u stanje karantina
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
ms.openlocfilehash: 0fc519c8170de498c9bcb1fc41a76116bda48b1f
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/04/2021
ms.locfileid: "50482902"
---
# <a name="workday-to-ad-user-provisioning-goes-into-quarantine-state"></a>Radni dan za obezbeđivanje oglasa korisnika ide u stanje karantina

**Radni dan za obezbeđivanje oglasa korisnika prelazi u stanje karantina i nijedan korisnik se ne kreira u OGLASU**

Radni dan za obezbeđivanje OGLAŠAVANJA za korisnika je otišao u stanje karantina, a evidentiranje nadzora prikazuje događaje izvoza pomoću greške sa porukom o grešci **: Operationser. Nije podešena nijedna superiorna referenca za uslugu direktorijuma. Usluga direktorijuma stoga ne može da izda referente objekte izvan ove šume**. Do ove greške obično dolazi ako kontejner Active Directory nije ispravno podešen ili ako postoje problemi sa mapiranjem izraza koje se koristi za **Parent.**

Potvrdite izbor u podrazumevanom dijalogu za **novi korisnici** parametra za Tipos. Uverite se da navedeno koje već postoji u vašem OGLASU. Ako koristite **Parent, Izhedime** u mapiranju atributa, uverite se da se uvek izračunava na poznat kontejner unutar domena oglasa. Pogledajte događaj izvoza u evidenciji nadzora da biste videli generisane vrednosti.

Za više detalja o konfigurisanju radnog vremena za automatizovano obezbeđivanje pogledajte [članak uputstvo: konfigurisanje radnog dana za automatsko obezbeđivanje korisnika](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).

