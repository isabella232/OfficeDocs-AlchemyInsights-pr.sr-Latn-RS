---
title: Identifikovanje događaja poruke u evidencijama nadzora
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
- "1370"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 7dd9c98bd45c29702fbc6cc14bf82bf7bce7d89d
ms.sourcegitcommit: 89d938a2d402791ae66dddadba3063e9418f48cb
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 07/28/2021
ms.locfileid: "53630083"
---
# <a name="audit-logs-for-deleted-email-messages"></a>Evidencije nadzora za izbrisane e-poruke

Počev od januara 2019, Microsoft podrazumevano uključiva evidentiranje nadzora poštanskog sandučeta. U suprotnom, da biste pregledali događaje brisanja poruka za određenog korisnika, morate ručno da omogućite radnje brisanja za nadzor. Ako je evidentiranje nadzora poštanskih sandučića već omogućeno za organizaciju ili za određenog korisnika, pratite korake u nastavku.

1. Prijavite se u [Microsoft 365 usaglašenosti](https://protection.office.com/)

2. Izaberite stavku **Pretraga i istraživanje,** a **zatim stavku Pretraga evidencije nadzora.**

3. Izaberite opseg datuma u poljima **Datum početka** i **Datum završetka.** Navedite korisničko ime za korisnika koje želite da istražite (korisnik koji je izbrisao stavke). U polju **Aktivnosti izaberite izbrisane** poruke iz **fascikle** "Izbrisane stavke" i Premeštene **poruke u fasciklu "Izbrisane stavke".**

4. Izaberite **stavku Pretraga**.

U rezultatima izaberite zapis nadzora. U iletu detalja izaberite stavku **Još informacija.** Dodatne informacije o izbrisanoj stavci (na primer, red za temu i lokaciju stavke kada je izbrisana) prikazuju se u polju Ugrožene **stavke.** Svojstvo **ClientInfoString** će prikazati ako se brisanje Outlook, Outlook na vebu (ranije poznato kao Outlook Web App) ili na bilo kom drugom uređaju.

Dodatne informacije potražite u [temi "Odlučivanje o tome ko je podesio prosleđivanje e-pošte za poštansko sanduče"](/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items).

**Napom:** Nije moguće preuzeti izbrisane stavke pomoću funkcije evidencije nadzora. Da biste preuzeli izbrisane poruke iz Outlook na vebu, pogledajte oporavak [izbrisanih stavki u Outlook Web App.](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4)
