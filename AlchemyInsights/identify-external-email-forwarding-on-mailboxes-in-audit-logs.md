---
title: Identifikovanje spoljnog prosleđivanja e-pošte na Poštanske sandučiće u evidenciji nadzora
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
ms.openlocfilehash: d06ef83adcae1342173a6fe75f79525c7e1797ce
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47696311"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>Identifikujte kada je spoljni Prosleđivanje e-pošte konfigurisan na poštanskim sandučićima

Kada Microsoft 365 korisnik konfiguriše spoljnu Prosleđivanje e-pošte u **poštansko sanduče,** aktivnost se nadgleda kao deo cmdlet adrese. Možete da vidite aktivnost pomoću pretrage evidencije nadzora u centru za bezbednost & bezbednosti.

1. Prijavite se u [Microsoft 365 Security & centar za usaglašenost](https://protection.office.com/).

2. Idite na stranicu **Search**  >  **Pretraga evidencije nadgledanja** za pretraživanje.

3. Izaberite opseg datuma u poljima **početni** i **Krajnji datum** . Nije potrebno da navedete korisničko ime. Proverite da li je polje **aktivnosti** podešeno da **prikazuje rezultate za sve aktivnosti**.

4. Kliknite na dugme **Pretraži**.

U rezultatima izaberite stavku **Filtriraj rezultate** i otkucajte **podešeno-poštansko sanduče** u polju Filter aktivnosti. Izaberite zapis nadzora u rezultatima. U okviru **Detalji** , kliknite na dugme **više informacija**. Morate da pogledate detalje o svakom zapisu nadzora da biste utvrdili da li je aktivnost povezana sa prosleđivanjem e-pošte.

- **ObjectId**: vrednost pseudonima koja je izmenjena u poštanskom sandučetu.

- **Parametri**: _forwardingsmtpadress_ pokazuje ciljnu e-adresu.

- **Korisnički ID**: korisnik koji konfiguriše Prosleđivanje e-pošte na poštansko sanduče u polju **ObjectId** .

Više informacija potražite u članku [Utvrđivanje ko je podesio Prosleđivanje e-pošte za poštansko sanduče](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox).
