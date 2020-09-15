---
title: Identifikovanje događaja brisanja poruka u evidenciji nadzora
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
ms.openlocfilehash: bc78076706aee15a3133c4b1a89064591f790b58
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47696527"
---
# <a name="audit-logs-for-deleted-email-messages"></a>Evidencija nadzora za izbrisane e-poruke

Počevši od januara 2019, Microsoft automatski pokreće Office proveru poštanskog sandučeta. U suprotnom, da biste pregledali brisanje događaja poruke za određenog korisnika, morate ručno da omogućite radnje brisanja za nadgledanje. Ako je evidentiranje nadzora poštanskog sandučeta već omogućeno za vašu organizaciju ili za određenog korisnika, slijedite dolenavedene korake.

1. Prijavite se u [Microsoft 365 Security & centar za usaglašenost](https://protection.office.com/)

2. Izaberite stavku **Pretraga i istraga** i izaberite stavku **Pretraga evidencije nadzora**.

3. Izaberite opseg datuma u poljima **početni** i **Krajnji datum** . Navedite korisničko ime za korisnika koga želite da istražite (korisnik koji je izbrisao stavke). U polju **aktivnosti** izaberite stavku **izbrisane poruke iz fascikle "Izbrisane stavke"** i **premestili poruke u fasciklu "Izbrisane stavke**".

4. Kliknite na dugme **Pretraži**.

U rezultatima izaberite zapis nadzora. U okviru detalji, kliknite na dugme **više informacija**. Dodatne informacije o izbrisanom artiklu (na primer, redu za temu i lokacija stavke kada je izbrisana) prikazuje se u polju " **Afekcteditem** ". **ClientInfoString** će se prikazati ako je brisanje došlo u programu Outlook, Outlook na vebu (ranije ime Outlook Web App) ili bilo kom drugom uređaju.

Više informacija potražite u članku [Utvrđivanje ko je podesio Prosleđivanje e-pošte za poštansko sanduče](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items).

**Napomena**: ne možete da preuzmete izbrisane stavke pomoću funkcije evidencije nadzora. Da biste preuzeli izbrisane poruke u programu Outlook na vebu, pogledajte članak [oporavak izbrisanih stavki u programu Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).
