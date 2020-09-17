---
title: Identifikovanje aktivnosti pravila prijemnog poštanskog sandučeta u evidenciji nadzora
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
ms.openlocfilehash: 3de6fcde6dc649cb77077d469cc66d4003e0c890
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/15/2020
ms.locfileid: "47779065"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a>Identifikovanje aktivnosti pravila prijemnog poštanskog sandučeta u evidenciji nadzora

Možete da koristite pretragu evidencije nadzora u Microsoft 365 Security & centar za usaglašenost da biste prikazali događaje pravila prijemnog poštanskog sandučeta (kreiranje, izmena i brisanje pravila prijemnog poštanskog sandučeta).

1. Prijavite se u [Microsoft 365 Security & centar za usaglašenost](https://protection.office.com/).

2. Idite na stranicu **Search**  >  **Pretraga evidencije nadgledanja** za pretraživanje.

3. Izaberite opseg datuma u poljima **početni** i **Krajnji datum** .

4. U okviru stavke **aktivnosti Exchange poštanskog sandučeta**potvrdite da je polje **aktivnosti** postavljeno na **novo-inboxpravilo kreiranje/izmena/omogućavanje/onemogućavanje pravila prijemnog poštanskog sandučeta**.

5. Kliknite na dugme **Pretraži**.

U rezultatima izaberite zapis nadzora. U okviru detalji, kliknite na dugme **više informacija**. Informacije o postavkama pravila prijemnog poštanskog sandučeta prikazuju se u polju **Parametri** .

Više informacija potražite u članku [Utvrđivanje toga da li je korisnik kreirao pravilo prijemnog poštanskog sandučeta](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)
