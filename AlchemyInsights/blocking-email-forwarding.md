---
title: 726 blokira Prosleđivanje e-pošte
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "726"
- "1200004"
ms.assetid: 8865c68e-7e8a-4135-a254-d7f69f1ded30
ms.openlocfilehash: c0d9ed14f83d3c7d47e1728d5ed9ca3a19412ad2
ms.sourcegitcommit: f74c9698a31634154ce58dda8b3145bb10685ace
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/23/2020
ms.locfileid: "48219869"
---
# <a name="blocking-or-unblocking-email-forwarding"></a>Blokiranje ili deblokiranje prosleđivanja e-pošte

Da biste omogućili ili onemogućili Prosleđivanje e-pošte za određeno poštansko sanduče, pogledajte članak [Konfigurisanje prosleđivanja e-pošte](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).

Na nivou zakupca kontrola spoljnog prosleđivanja se obavlja pomoću izlazne smernice za borbu protiv bezvredne pošte. Ako je podešena na stavku isključeno ili automatski, to može da blokira Prosleđivanje e-pošte pomoću stavke "550 5.7.520 pristup nije dozvoljen, organizacija ne dozvoljava grešku spoljne prosleđivanja". Zatim, ako je podešeno da bude blokirano, to je greška koju će korisnici videti.

Ako je prosleđivanje blokirano, proverite da li su smernice konfigurisane tako da omogućavaju eksterni Autonapred. Možete da potvrdite smernice za filtriranje odlazne bezvredne pošte iz centra za bezbednost i usaglašenost ili tako što ćete pokrenuti komandnu karticu. ime za for, Autoforwardingmod. Ako želite da podesite automatsko blokiranje, ista komanda će vam odmah reći stanje politike.

Napomena: preporučuje se da spoljna automatska funkcija ostane sprečena u podrazumevanim smernicama za izlazne količine i omogućite samo za korisnike kojima je potrebna spoljna prosleđivanje kreiranjem prilagođenih smernica za te korisnike. Možete pročitati više o [konfigurisanju spoljnog prosleđivanja e-pošte u sistemu Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).