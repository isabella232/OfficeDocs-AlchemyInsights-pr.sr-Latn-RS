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
ms.openlocfilehash: 3bda32b55be9c2fa671376e73b06aadfbe976363
ms.sourcegitcommit: 89d938a2d402791ae66dddadba3063e9418f48cb
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 07/28/2021
ms.locfileid: "53630191"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a>Identifikovanje aktivnosti pravila prijemnog poštanskog sandučeta u evidencijama nadzora

Pretragu evidencije nadzora možete da koristite u Microsoft 365 centru za bezbednost & za usaglašenost da biste prikazali događaje pravila prijemnog poštanskog sandučeta (kreiranje, izmenu i brisanje pravila prijemnog poštanskog sandučeta).

1. Prijavite se u Microsoft 365 [za usaglašenost.](https://protection.office.com/)

2. Idite na stranicu  >  **Pretraga evidencije nadzora pretrage.**

3. Izaberite opseg datuma u poljima **Datum početka** i **Datum završetka.**

4. U **Exchange** aktivnosti poštanskog sandučeta  proverite da li je polje Aktivnosti postavljeno na Opciju Novo prijemno poštansko **sandučeRule Kreiranje/izmena/omogućavanje/onemogućavanje pravila prijemnog poštanskog sandučeta.**

5. Izaberite **stavku Pretraga**.

U rezultatima izaberite zapis nadzora. U iletu detalja izaberite stavku **Još informacija.** Informacije o postavkama pravila prijemnog poštanskog sandučeta prikazuju se u polju **Parametri.**

Dodatne informacije potražite u [temi "Odlučivanje da li je korisnik napravio pravilo prijemnog poštanskog sandučeta"](/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)
