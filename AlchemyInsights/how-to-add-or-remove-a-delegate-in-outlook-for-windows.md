---
title: Dodavanje ili uklanjanje delegata u programu Outlook za Windows
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3800004"
- "7334"
ms.openlocfilehash: fcbd6082c104f0e1bca022a23cbbeb6e3363a6c5
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573572"
---
# <a name="how-to-add-or-remove-a-delegate-in-outlook-for-windows"></a>Dodavanje ili uklanjanje delegata u programu Outlook za Windows

Da biste dodali delegata u programu Outlook za Windows: 

1. Kliknite na karticu **datoteka** pored stavke **Postavke naloga**, a zatim odaberite stavku **Delegirani pristup**.
2. Kliknite na dugme " **Dodaj**". Ako se **Add** ne pojavi, aktivna veza možda ne postoji između Outlook i Exchange servera. Outlook statusna traka prikazuje status veze.
3. Otkucajte ime osobe koju želite da odredite kao delegata ili pretražite i odaberite ime na listi rezultata pretrage.

    > [!NOTE]
    > Delegat mora da bude osoba na Exchange globalnom spisku adresa (GAL) organizacije.
4. Kliknite na dugme " **Dodaj** ," u **redu**.
5. U dijalogu **delegirane dozvole** prihvatite podrazumevane postavke dozvole ili izaberite stavku prilagođeni nivoi pristupa za Exchange fascikle.

    - Ako delegatu treba dozvola za rad samo sa pozivima za sastanke i odgovorima, podrazumevane postavke dozvola kao što je **Delegat prima kopije poruka koje su mi poslate u vezi sa sastankom** . Možete da ostavite postavke dozvole **prijemnog poštanskog sandučeta** na **nijedan**. Pozivi za sastanak i odgovori će otići direktno u prijemno poštansko sanduče delegata.

    > [!NOTE]
    > Podrazumevano, delegat se dodeljuje dozvola za **Uređivanje (može da čita, kreira i menja stavke)** u fascikli " **Kalendar** ". Kada delegat odgovori na sastanak u vaše ime, on se automatski dodaje u fasciklu " **Kalendar** ".

5. Da biste poslali poruku da obavestite delegata za promenjene dozvole, potvrdite izbor u polju za potvrdu **automatski Pošalji poruku delegatu za rezimiranje ovih dozvola** .
6. Ako želite, potvrdite izbor u polju za potvrdu **Delegat može da vidi moje privatne stavke** .

    > [!IMPORTANT]
    > Ova postavka utiče na sve Exchange fascikle. To obuhvata sve e-poštu, kontakte, kalendare, zadatke, beleške i fascikle naloga. Ne postoji način za odobravanje pristupa privatnim stavkama u samo navedenim fasciklama.

7. Odaberite stavku **u redu**.

    > [!NOTE]
    >
    > - Poruke poslate sa **dozvolama "Pošalji** u ime" sadrže dozvole delegata i vaša imena pored. Kada se poruka pošalje sa dozvolama "Pošalji kao", pojavljuje se samo vaše ime.
    > - Kada dodate nekog kao delegata, može da doda Exchange poštansko sanduče u Outlook profil. Uputstva potražite u članku [upravljanje stavkama pošte i kalendara druge osobe](https://support.microsoft.com/office/manage-another-person-s-mail-and-calendar-items-afb79d6b-2967-43b9-a944-a6b953190af5).

Da biste uklonili delegata u programu Outlook za Windows:

1. Kliknite na karticu **datoteka** .
2. Izaberite stavku **Postavke naloga** , a zatim **Delegirani pristup**.
3. Odaberite ime delegata za koga želite da promenite dozvole, a zatim kliknite na dugme **Ukloni** , a zatim **u redu**.
