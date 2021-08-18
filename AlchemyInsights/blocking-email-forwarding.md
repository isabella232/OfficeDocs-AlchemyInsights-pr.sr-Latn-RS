---
title: Blokiranje ili deblokiranje spoljnog automatskog prosleđivanja e-pošte
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
ms.openlocfilehash: fe9e52023b809b38c43332a10a1184d114798cfe
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/13/2021
ms.locfileid: "58315888"
---
# <a name="block-or-unblock-eternal-automatic-email-forwarding"></a>Blokiranje ili deblokiranje automatskog prosleđivanja e-pošte

Da biste omogućili ili onemogućili prosleđivanje e-pošte za određeno poštansko sanduče, pogledajte [konfigurisanje prosleđivanja e-pošte.](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding)

Administracioni programi mogu da kontrolišu spoljno prosleđivanje za organizaciju pomoću [smernica za odlaznu bezb.](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-outbound-spam-policy) Smernicama za odlaznu bezvrednu e-Microsoft 365 zaštitnik na Microsoft 365 zaštitnik portalu ili pomoću <https://security.microsoft.com/antispam> [Get-HostedOutboundSpamFilterPolicy](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy) cmdlet u programu Exchange Online PowerShell.

Ako dobijete sledeću grešku: **"550 5.7.520 Pristup** odbijen, vaša organizacija ne dozvoljava spoljno prosleđivanje" , uverite se da su smernice konfigurisane tako da omogućavaju spoljno automatsko prosleđivanje poruka.

Napomi: Preporučujemo  podrazumevanu vrednost Automatsko  – Sistem se kontroliše za postavku Pravila za automatsko prosleđivanje u podrazumevanim smernicama filtera odlazne bez pošte (automatsko spoljno prosleđivanje je blokirano; interno automatsko prosleđivanje i dalje funkcioniše).  Trebalo bi da kreirate prilagođene smernice za filtriranje odlazne pošte i da koristite vrednost On **– Prosleđivanje** je omogućeno samo za korisnike kojima je potrebno spoljno automatsko prosleđivanje e-pošte. Dodatne informacije potražite u [temi Konfigurisanje spoljnog prosleđivanja e-pošte u Office 365.](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding)
