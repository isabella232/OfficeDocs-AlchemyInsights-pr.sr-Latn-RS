---
title: Identifikovanje spoljnog prosleđivanja e-pošte u poštanskim sandučićima u evidencijama nadzora
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
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 48634fad8f573e3a7c38cac299bb95ec90814f5c
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/13/2021
ms.locfileid: "58331173"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>Identifikovanje kada je spoljno prosleđivanje e-pošte konfigurisano u poštanskim sandučićima

Kada Microsoft 365 konfiguriše spoljno prosleđivanje e-pošte u poštanskom sandučetu, aktivnost se nadgleda kao deo cmdlet stavke **Set-Mailbox** cmdlet. Aktivnost možete da vidite pomoću pretrage evidencije nadzora. Evo kako to da uradite.

1. Uradite nešto od sledećeg:
   - U e-Microsoft 365 centar za usaglašenost <https://compliance.microsoft.com> , idite na Nadzor  \> **rešenja**. Ili, da biste direktno prešli na **stranicu Nadzor,** koristite <https://compliance.microsoft.com/auditlogsearch> .
   - Na portalu Microsoft 365 zaštitnik , <https://security.microsoft.com> idite na Nadzor . Ili, da biste direktno prešli na **stranicu Nadzor,** koristite <https://sip.security.microsoft.com/auditlogsearch> .

2. Na stranici **Nadzor** potvrdite da je **izabrana** kartica Pretraga, a zatim konfigurišite sledeće postavke:
   - Izaberite opseg datuma/vremena u **pocima Početak** **i** Kraj.
   - Potvrdite **da polje Aktivnosti** sadrži **opciju Prikaži rezultate za sve aktivnosti.**

3. Kada završite, kliknite na dugme **Pretraži**. Aktivnosti se pojavljuju na novoj stranici **Pretraga nadzora.**

4. U rezultatima izaberite stavku **Filtriraj rezultate** i **otkucajte Set-Mailbox** u polju filtera aktivnosti.

5. Izaberite zapis nadzora u rezultatima. Na **iletu "Detalji"** kliknite na dugme **"Više informacija"**. Morate da pogledate detalje svakog zapisa nadzora da biste utvrdili da li je aktivnost povezana sa prosleđivanju e-pošte.

   - **ObjectId:** Pseudonim vrednosti poštanskog sandučeta koje je izmenjeno.
   - **Parametri:** _ForwardingSmtpAddress ukazuje_ na ciljnu e-adresu.
   - **UserId:** Korisnik koji je konfigurovao prosleđivanje e-pošte u poštanskom sandučetu u **polju ObjectId.**

Dodatne informacije potražite u [temi "Odlučivanje o tome ko je podesio prosleđivanje e-pošte za poštansko sanduče"](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox).
