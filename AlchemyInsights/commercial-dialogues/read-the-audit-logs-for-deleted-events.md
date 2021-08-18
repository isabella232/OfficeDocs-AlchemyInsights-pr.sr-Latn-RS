---
title: Čitanje evidencija nadzora za izbrisane događaje
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: ec8f845f599e397814bc9077c3fe59edb5324192
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/13/2021
ms.locfileid: "58324747"
---
# <a name="read-the-audit-logs-for-deleted-events"></a>Čitanje evidencija nadzora za izbrisane događaje

Evo kako to da uradite:

1. Uradite nešto od sledećeg:
   - Na Microsoft 365 centar za usaglašenost <https://compliance.microsoft.com> , idite na Nadzor  \> **rešenja**. Ili, da biste direktno prešli na **stranicu Nadzor,** koristite <https://compliance.microsoft.com/auditlogsearch> .
   - Na portalu Microsoft 365 zaštitnik , <https://security.microsoft.com> idite na Nadzor . Ili, da biste direktno prešli na **stranicu Nadzor,** koristite <https://security.microsoft.com/auditlogsearch> .

    **Napomi:** Ako vidite obaveštenje da morate da uključite funkciju, uključite je odmah. Ako funkcija nije uključena, rezultati pretrage neće moći da povlače podatke iz prethodnih datuma.

2. Na **kartici Pretraga** na **stranici** Nadzor konfigurišite sledeće postavke:
   - **Opseg datuma i vremena:** Izaberite opseg datum/vreme u pocima **Početak** **i** Kraj.
   - **Aktivnosti:** Unesite **Exchange poštanskog sandučeta,** a zatim izaberite sledeće vrednosti:
     - **Izbrisane poruke iz fascikle "Izbrisane stavke"**
     - **Premeštene poruke u fasciklu "Izbrisane stavke"**

       Kada završite, kliknite izvan okna da biste umanjili **okno Aktivnosti.**

   - **Korisnici:** Prihvatite praznu podrazumevanu vrednost da biste vratili rezultate za sve korisnike ili unesite jednog korisnika ili više njih.

3. Kada završite, kliknite na dugme **Pretraži**. Aktivnosti se pojavljuju na novoj stranici **Pretraga nadzora.**

4. Izaberite aktivnost u rezultatima da biste otvorili letak sa detaljima. Dodatne informacije o izbrisanoj stavci, kao što su red za temu i lokacija stavke kada je izbrisana, prikazuju se u polju Ugrožene **stavke.**

   **Napoma:** Nije moguće vratiti izbrisane stavke pomoću funkcije evidencije nadzora. Da biste vratili izbrisane stavke, pogledajte [oporavak izbrisanih e-poruka u Outlook na vebu.](https://support.microsoft.com/office/recover-deleted-email-messages-in-outlook-on-the-web-a8ca78ac-4721-4066-95dd-571842e9fb11)

Više informacija potražite u video zapisu [Pretraga evidencije nadzora da biste istražili uobičajene probleme sa podrškom.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios)
