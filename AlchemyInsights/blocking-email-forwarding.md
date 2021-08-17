---
title: 726 Blokiranje prosleđivanja e-pošte
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
ms.openlocfilehash: 0bff7ede02809e133dc6616452ec840f552bd4fa6c45b7987d6455b2a9ba49bf
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "54059646"
---
# <a name="blocking-or-unblocking-email-forwarding"></a>Blokiranje ili deblokiranje prosleđivanja e-pošte

Da biste omogućili ili onemogućili prosleđivanje e-pošte za određeno poštansko sanduče, pogledajte konfigurisanje [prosleđivanja e-pošte.](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding)

Na nivou zakupca, kontrola spoljnog prosleđivanja se pravi pomoću smernica za odlaznu bez-e-pošti. Smernice za filtriranje odlazne bez pošte [](https://protection.office.com/antispam) možete da pogledate iz centra za bezbednost i usaglašenost ovde ili pomoću komande [Get-HostedOutboundSpamFilterPolicy.](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy)

Ako dobijate sledeću grešku: **"550 5.7.520 Access** je odbijen, vaša organizacija ne dozvoljava spoljno prosleđivanje" , uverite se da je smernica konfigurisana tako da omogućava spoljno automatsko prosleđivanje.

**Napomogućeno:** Preporučuje se da se spoljna usluga automatskog osveženja onemogući na podrazumevanoj smernici filtera odlazne bezvredne pošte i omogući samo za korisnike kojima je potrebno spoljno prosleđivanje kreiranjem prilagođenih smernica za te korisnike. Možete da pročitate više u [temi Konfigurisanje spoljnog prosleđivanja e-pošte u Office 365.](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding)