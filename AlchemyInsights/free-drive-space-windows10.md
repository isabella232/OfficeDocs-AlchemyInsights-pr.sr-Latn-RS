---
title: Oslobodite prostor za disk jedinicu u operativnom sistemu Windows 10
ms.author: pebaum
author: pebaum
manager: dansimp
ms.date: 03/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9771"
- "9005403"
ms.openlocfilehash: 3838f3db3bc5f54bcb1a2558484056f3194b76e1
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037947"
---
# <a name="free-up-drive-space-in-windows-10"></a>Oslobodite prostor za disk jedinicu u operativnom sistemu Windows 10

Evo dve opcije da biste oslobodili prostor za disk jedinicu u operativnom sistemu Windows:

- Oslobodite prostor za disk jedinicu u operativnom sistemu Windows 10.
- Oslobodite prostor za Windows 10 ispravke sa spoljnim uređajem za skladištenje.

Ako i dalje imate nizak prostor na disku nakon korišćenja alatke "Čišćenje diska", moguće je da se fascikla temp brzo popunjava sa datotekama aplikacije (. appx) koje koristi Microsoft Store. Da biste rešili ovaj problem, poništite skladište, obrišite keš skladišta, a zatim pokrenite alatku za rešavanje problema sa uslugom Windows Update. Uverite se da je Microsoft prodavnica zatvorena pre nego što nastavite sa ovim koracima.

**1. prvi: poništavanje Microsoft prodavnice**

**Napomena** Ovo trajno briše podatke aplikacije na uređaju, uključujući željene postavke i detalje za prijavljivanje.

1. Izaberite stavke postavke **početnog**  >  **postavki**  >    >  **& funkcijama**.

1. Na listi aplikacija pronađite i izaberite stavku Microsoft butik.

1. Izaberite stavku **Napredne opcije**.

1. Pomerajte se nadole i izaberite stavku **Poništi**, a zatim **potvrdite početne vrednosti**.

**2.2: Opozovite izbor u okviru keš Microsoft prodavnice**

1. Pritisnite taster sa Windows logotipom + R da biste otvorili dijalog "pokreće".

1. Otkucajte wsreset.exe i kliknite na **dugme u redu**.

1. Otvara se prazan prozor komandne linije. Posle 10 sekundi, prozor se zatvara i automatski se otvara.

**Treći broj: poništi Windows Update**

1. Izaberite stavku **pokretanje**  >  **postavki**  >  **Ažuriranje & bezbednosti**  >  .

1. Pomerajte se nadole i izaberite stavku **Windows Update** sa liste i izaberite stavku **pokrenite alatku za rešavanje problema**.

1. Ponovo pokrenite računar i provjerite da li i dalje nailazite na problem.

