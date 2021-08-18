---
title: Identifikovanje aktivnosti pravila prijemnog poštanskog sandučeta u evidencijama nadzora
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1368"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 1f252836d624b4550e1f3c87cf4fd7309dec6e91
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/13/2021
ms.locfileid: "58331137"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a>Identifikovanje aktivnosti pravila prijemnog poštanskog sandučeta u evidencijama nadzora

Možete da koristite pretragu evidencije nadzora u programu Microsoft 365 centar za usaglašenost za prikazivanje događaja pravila prijemnog poštanskog sandučeta (kreiranje, menjanje i brisanje pravila prijemnog poštanskog sandučeta).

1. Uradite nešto od sledećeg:
   - U e-Microsoft 365 centar za usaglašenost <https://compliance.microsoft.com> , idite na Nadzor  \> **rešenja**. Ili, da biste direktno prešli na **stranicu Nadzor,** koristite <https://compliance.microsoft.com/auditlogsearch> .
   - Na portalu Microsoft 365 zaštitnik , <https://security.microsoft.com> idite na Nadzor . Ili, da biste direktno prešli na **stranicu Nadzor,** koristite <https://security.microsoft.com/auditlogsearch> .

2. Na **kartici Pretraga** na **stranici** Nadzor konfigurišite sledeće postavke:
   - **Opseg datuma i vremena:** Izaberite opseg datum/vreme u pocima **Početak** **i** Kraj.
   - **Aktivnosti:** Izaberite jednu ili više od sledećih vrednosti:
     - **New-InboxRule Kreiranje pravila prijemnog poštanskog sandučeta od Outlook Web App**
     - **Set-InboxRule Izmenite pravilo iz Outlook Web App**.
     - **Ažuriranje pravila za prijemno poštansko sanduče Outlook klijenta**

3. Kada završite, kliknite na dugme **Pretraži**. Aktivnosti se pojavljuju na novoj stranici **Pretraga nadzora.**

4. Izaberite aktivnost u rezultatima da biste otvorili letak sa detaljima. Informacije o postavkama pravila prijemnog poštanskog sandučeta prikazuju se u **polju Parametri.**

Dodatne informacije potražite u [temi Odlučivanje o tome da li je korisnik napravio pravilo prijemnog poštanskog sandučeta.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-created-an-inbox-rule)
