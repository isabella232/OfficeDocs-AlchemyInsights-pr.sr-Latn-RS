---
title: 2491 Obaveštenje o e-porukama od smernica "Phish Delivered due to tenant or user override"
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2491
ms.assetid: ''
ms.openlocfilehash: 90b078147bbb1e60cba0a2de6e49a862469f93aa
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/13/2021
ms.locfileid: "58316372"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a>Upozorenje e-poruka iz smernica "Phish Delivered due to zakupca ili user override"

Podrazumevana smernica za obaveštenja koja se zove **Phish Delivered** zbog zamene zakupca ili korisnika dostupna je u organizacijama koje imaju licence za programe Microsoft zaštitnik za licence za Office 365 P1 i P2. Ako ste dobili ovo obaveštenje, evo koraka koje treba da istražite:

1. U poruci upozorenja izaberite **stavku Prikaži obaveštenje** da biste **prešli** na stranicu Obaveštenja na Microsoft 365 zaštitnik portalu.

2. Izaberite obaveštenje da biste videli opciju Prikaži **listu poruka ili Prikaži** poruke u **programu Explorer.** Obe ove opcije će vas odvesti do detalja poruke koja sadrži ID poruke. Imajte napom da će veza "Istraživač pretnji" automatski filtrirati poruke koje ispunjavaju kriterijume upozorenja. Možda ćete morati da prilagodite filter datuma u programu Threat Explorer.

Phishing poruka je isporučena zbog ručno konfigurisane zamene:

- Dozvoljeni pošiljalac ili domen koji je postavio korisnik.
- Dozvoljenog pošiljaoca ili domena koje je postavio administraator u smernicama za borbu protiv spam e-pošiljke.
- Dozvoljena IP adresa u smernicama filtera veze.
- Pravilo protoka pošte (poznato i kao pravilo za prenos) koje je konfigurisano tako da dozvoljava slanje poruka.

Ako smatrate da je poruka pogrešno označena kao phishing, koristite [prosleđivanje "Admin"](https://docs.microsoft.com/microsoft-365/security/office-365-security/admin-submission) da biste prijavili poruku korporaciji Microsoft.

Korisnici mogu da koriste programski dodatak "Poruka izveštaja" ili programski dodatak "Izveštaj o [phishingu"](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) Outlook da bi prosledili uzorke poruka korporaciji Microsoft.
