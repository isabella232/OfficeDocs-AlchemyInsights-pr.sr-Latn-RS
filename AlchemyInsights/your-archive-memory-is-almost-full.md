---
title: Poštansko sanduče arhive je gotovo popunjeno
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100006"
- "7960"
ms.openlocfilehash: 5c7081f8991716a8ac72f462c6c7ef88e800ab9c
ms.sourcegitcommit: 6f1af4aed507d4c074c36d77666cf00100efe168
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974662"
---
# <a name="your-archive-mailbox-is-almost-full"></a>Poštansko sanduče arhive je gotovo popunjeno

Ako korisnik prima upozorenje; **Poštansko sanduče arhive je gotovo popunjeno** ili treba da povećate veličinu njihovog poštanskog sandučeta, evo nekih saveta:

1. Ako je korisniku dodeljen Exchange online plan 1, nadogradite licencu **online plan 2** da biste povećali veličinu od 50 GB do 100gb.
1. Ako je korisniku već dodeljen neki od sledećih radnji: **Exchange online plan 2** ili Exchange online plan 1 pomoću programskog dodatka Exchange online arhiv za arhiviranje, koristite dolenavedene korake da biste omogućili automatsko proširivanje:.
 
    1. [Povezivanje sa uslugom Exchange online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true).
    2. Koristite sledeće zapovesti za korisnika:  `Enable-Mailbox <user mailbox> -AutoExpandingArchive`
    1. Uradite sledeće zapovjeli da biste potvrdili da je omogućena za korisnika:  `Get-Mailbox <user mailbox> | FL AutoExpandingArchiveEnabled`

Više informacija potražite u članku:

- [ Omogućavanje neograničene arhiviranja-administratorske pomoći-Microsoft 365 usaglašenost | Microsoft docs](https://docs.microsoft.com/microsoft-365/compliance/enable-unlimited-archiving?view=o365-worldwide&preserve-view=true)

- [Exchange online ograničenja – opisi usluge | Microsoft docs](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits?redirectedfrom=MSDN#storage-limits-across-standalone-plans)

- [Nadogradnja na drugačiji poslovni plan | Microsoft docs](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan?view=o365-worldwide&preserve-view=true)

