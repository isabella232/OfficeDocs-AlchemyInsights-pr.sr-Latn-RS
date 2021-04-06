---
title: Oslobađanje prostora na disk jedinici na OS Windows 10
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
- "9774"
- "9005390"
- "9005403"
ms.openlocfilehash: 2313636307bfddce2810c2d4c4ce9e3b407a7bdf
ms.sourcegitcommit: 7b2e5078dd65f11af6650e692a7ea48e91f544e0
ms.translationtype: HT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/02/2021
ms.locfileid: "51505370"
---
# <a name="free-up-drive-space-in-windows-10"></a>Oslobađanje prostora na disk jedinici na OS Windows 10

Ovo su dve opcije za oslobađanje prostora na disk jedinici na OS Windows:

- Oslobodite prostor na disk jedinici na OS Windows 10.
- Oslobodite prostor za Windows 10 ispravke sa spoljnim uređajem za skladištenje.

Ako i dalje nemate dovoljno prostora na disku nakon čišćenja diska, moguće je da se fascikla privremenih datoteka brzo puni datotekama aplikacija (.appx) koje koristi Microsoft Store prodavnica. Da biste rešili ovaj problem, resetujte Store prodavnicu, obrišite keš memoriju Store prodavnice, a zatim pokrenite rešavanje problema veb lokacije Windows Update. Proverite da li je Microsoft Store prodavnica zatvorena pre nego što nastavite sa ovim koracima.

**1. korak: Resetujte Microsoft Store**

**Napomena** Ovo trajno briše podatke aplikacija na uređaju, uključujući i željene postavke i detalje o prijavljivanju.

1. Izaberite **ekran „Početak“** > **Postavke** > **Aplikacije** > **Aplikacije i funkcije**.

1. Na listi aplikacija pronađite i izaberite Microsoft Store prodavnicu.

1. Izaberite **Napredne opcije**.

1. Pomerajte se nadole i izaberite stavku **Resetovanje**, a zatim stavku **Potvrdi resetovanje**.

**2. korak: Obrišite keš memoriju Microsoft Store prodavnice**

1. Pritisnite kombinaciju tastera sa Windows logotipom + R da biste otvorili dijalog „Pokretanje“.

1. Otkucajte wsreset.exe i izaberite stavku **U redu**.

1. Otvara se prazan prozor komandne linije. Nakon oko 10 sekundi, prozor se zatvara a Store prodavnica se automatski otvara.

**3. korak: Resetovanje veb lokacije Windows Update**

1. Izaberite **ekran „Početak“** > **Postavke** > **Ažuriranje i bezbednost** > **Rešavanje problema**.

1. Krećite se nadole i izaberite stavku **Veb lokacija Windows Update** sa liste, a zatim izaberite stavku **Pokreni rešavanje problema**.

1. Ponovo pokrenite računar i proverite da li se problem i dalje javlja.

