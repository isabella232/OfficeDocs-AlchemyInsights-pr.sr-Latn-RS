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
ms.openlocfilehash: b7146b2b09b6ac1e33b192dcbcbfb72ea2593313
ms.sourcegitcommit: 89d938a2d402791ae66dddadba3063e9418f48cb
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 07/28/2021
ms.locfileid: "53630263"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>Identifikovanje kada je spoljno prosleđivanje e-pošte konfigurisano u poštanskim sandučićima

Kada korisnik Microsoft 365 spoljno prosleđivanje e-pošte u poštanskom sandučetu, aktivnost se nadgleda kao deo cmdlet stavke **Set-Mailbox** cmdlet. Aktivnost možete da vidite pomoću pretrage evidencije nadzora u centru & za usaglašenost.

1. Prijavite se u Microsoft 365 [za usaglašenost.](https://protection.office.com/)

2. Idite na stranicu  >  **Pretraga evidencije nadzora pretrage.**

3. Izaberite opseg datuma u poljima **Datum početka** i **Datum završetka.** Ne morate da navodite korisničko ime. Potvrdite **da je polje Aktivnosti** podešeno na prikaži **rezultate za sve aktivnosti.**

4. Izaberite **stavku Pretraga**.

U rezultatima izaberite stavku **Filtriraj rezultate** i **otkucajte Set-Mailbox** u polju filtera aktivnosti. Izaberite zapis nadzora u rezultatima. Na **iletu "Detalji"** kliknite na dugme **"Više informacija"**. Morate da pogledate detalje svakog zapisa nadzora da biste utvrdili da li je aktivnost povezana sa prosleđivanju e-pošte.

- **ObjectId:** Pseudonim vrednosti poštanskog sandučeta koje je izmenjeno.

- **Parametri:** _ForwardingSmtpAddress ukazuje_ na ciljnu e-adresu.

- **UserId:** Korisnik koji je konfigurovao prosleđivanje e-pošte u poštanskom sandučetu u **polju ObjectId.**

Dodatne informacije potražite u [temi "Odlučivanje o tome ko je podesio prosleđivanje e-pošte za poštansko sanduče"](/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox).
