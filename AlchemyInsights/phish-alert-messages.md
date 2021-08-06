---
title: 2491 Obaveštenje e-poruka od smernica "Phish Delivered due to tenant or user override"
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
ms.openlocfilehash: ac4c157d6e202488659c56605768bbfd2b3af8e658d0a2f82e529fdac6763fa9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "53999686"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a>Upozorenje e-poruka iz smernica "Phish Delivered due to zakupca ili user override"

Podrazumevane smernice za obaveštenja "Phish Delivered due to tenant or user override" dostavljaju se zakupcima koji imaju licence za Office 365 P1 i P2. Ako ste dobili ovo obaveštenje, evo koraka koje treba da istražite:

1. U poruci upozorenja izaberite stavku  **Prikaži obaveštenje** da biste prešli na stranicu Obaveštenja u centru za & za usaglašenost.

2. Izaberite obaveštenje da biste videli opciju Prikaži **listu poruka ili Prikaži** poruke u **programu Explorer.** Obe ove opcije će vas odvesti do detalja poruke koja sadrži ID poruke. Imajte napom da će veza "Istraživač pretnji" automatski filtrirati poruke koje ispunjavaju kriterijume upozorenja. Možda ćete morati da prilagodite filter datuma u programu Threat Explorer.

Phishing poruka je isporučena zbog ručno konfigurisane zamene:

- Dozvoljeni pošiljalac ili domen koji je postavio korisnik.

- Dozvoljenog pošiljaoca ili domena koje je postavio administratovani pošiljalac u smernicama za borbu protiv spam e-pošiljke.

- Dozvoljena IP adresa u smernicama filtera veze.

- Pravilo protoka pošte (poznato i kao pravilo za prenos) koje je konfigurisano tako da dozvoljava slanje poruka.

Ako smatrate da je poruka pogrešno označena kao phish, koristite programski dodatak Outlook [Report Message](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) da biste prosledili uzorke poruka korporaciji Microsoft.
