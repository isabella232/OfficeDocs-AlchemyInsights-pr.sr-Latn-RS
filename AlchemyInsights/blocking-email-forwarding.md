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
ms.openlocfilehash: 610013c4f46e999f1a8715aea14dd557ed8b0e2a
ms.sourcegitcommit: 88f24bb6ced16842de165af416e3f21feae13063
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 10/15/2020
ms.locfileid: "48478311"
---
# <a name="blocking-or-unblocking-email-forwarding"></a>Blokiranje ili deblokiranje prosleđivanja e-pošte

Da biste omogućili ili onemogućili Prosleđivanje e-pošte za određeno poštansko sanduče, pogledajte članak [Konfigurisanje prosleđivanja e-pošte](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).

Na nivou zakupca kontrola spoljnog prosleđivanja se obavlja pomoću izlaznih smernica bezvredne pošte. Možete da potvrdite [izbor u](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy)polju za proveru izlaznih polja bezvredne pošte iz [centra za](https://protection.office.com/antispam) bezbednost i usaglašenost

Ako dobijate sledeću grešku: **"550 5.7.520 pristup je odbijen, organizacija ne dozvoljava spoljne prosleđivanje"**, proverite da li su smernice konfigurisane tako da omogućuju spoljni automatski pristup.

**Napomena:** Preporučuje se da spoljna automatska funkcija ostane sprečena u podrazumevanim smernicama za izlaznu vrednost izlaznog bezvredne pošte i da je omogućite samo za korisnike kojima je potrebna spoljna prosleđivanje kreiranjem prilagođenih smernica za te korisnike. Možete pročitati više o [konfigurisanju spoljnog prosleđivanja e-pošte u sistemu Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).