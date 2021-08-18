---
title: Istraživanje svih aktivnosti korisnika
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002486"
- "7524"
ms.openlocfilehash: 016f4b1caa05cb26d1e6795551b64737d4cb64a5
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/13/2021
ms.locfileid: "58332357"
---
# <a name="investigate-all-the-users-activities"></a>Istraživanje svih aktivnosti korisnika

Evo kako to da uradite:

1. Uradite nešto od sledećeg:
   - U e-Microsoft 365 centar za usaglašenost <https://compliance.microsoft.com> , idite na Nadzor  \> **rešenja**. Ili, da biste direktno prešli na **stranicu Nadzor,** koristite <https://compliance.microsoft.com/auditlogsearch> .
   - Na portalu Microsoft 365 zaštitnik , <https://security.microsoft.com> idite na Nadzor . Ili, da biste direktno prešli na **stranicu Nadzor,** koristite <https://security.microsoft.com/auditlogsearch> .

    **Napomi:** Ako vidite obaveštenje da morate da uključite funkciju, uključite je odmah. Ako funkcija nije uključena, rezultati pretrage neće moći da povlače podatke iz prethodnih datuma.

2. Na **kartici Pretraga** na **stranici** Nadzor konfigurišite sledeće postavke:
   - **Opseg datuma i vremena:** Izaberite opseg datum/vreme u pocima **Početak** **i** Kraj.
   - **Aktivnosti:** Ako ste zainteresovani za određenu aktivnost, izaberite je sa liste; u suprotnom, **podrazumevana vrednost Prikaži rezultate za** sve aktivnosti vraća sve aktivnosti.
   - **Korisnici:** Prihvatite praznu podrazumevanu vrednost da biste vratili rezultate za sve korisnike ili unesite jednog korisnika ili više njih.

3. Kada završite, kliknite na dugme **Pretraži**. Aktivnosti se pojavljuju na novoj stranici **Pretraga nadzora.** Videćete **IP adresu,** **korisničko ime** i **ime** aktivnosti.

4. Da biste preuzeli  rezultate, izaberite stavku \> **Izvezi preuzimanje svih rezultata.**

5. Izaberite aktivnost u rezultatima da biste otvorili letak sa detaljima.

Da biste saznali više, pogledajte pretragu [evidencije nadzora da biste istražili uobičajene probleme sa podrškom.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios)
