---
title: Arhiviranje poštanskog sandučeta je skoro puno
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
ms.openlocfilehash: 085d9b211d5a8e9a0e1eb12af14d87a4e59c844a3afa012095dfd60db316ad14
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "54046766"
---
# <a name="your-archive-mailbox-is-almost-full"></a>Arhiviranje poštanskog sandučeta je skoro puno

Ako korisnik dobije upozorenje; **Arhivno poštansko sanduče je skoro puno** ili treba da povećate veličinu njihovog arhivnog poštanskog sandučeta, evo nekih saveta:

1. Ako se korisniku dodelite Exchange Online Plan 1, nadogradite ga na **Exchange Online Plan 2** da biste povećali veličinu sa 50 GB na 100 GB.
1. Ako je korisniku već dodeljeno nešto od sledećeg: **Exchange Online Plan 2** ili Exchange Online Plan 1 uz Exchange Online arhiviranje dodatak, koristite dolenavodene korake da biste omogućili automatsko razvijanje arhiviranje:.
 
    1. [Povezivanje da Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true).
    2. Pokrenite sledeću komandu za korisnika:  `Enable-Mailbox <user mailbox> -AutoExpandingArchive`
    1. Pokrenite sledeću komandu da biste potvrdili da je omogućena za korisnika:  `Get-Mailbox <user mailbox> | FL AutoExpandingArchiveEnabled`

Više informacija potražite u:

- [Omogućavanje neograničenog arhiviranje – pomoć za Microsoft 365 za | Microsoft Docs](https://docs.microsoft.com/microsoft-365/compliance/enable-unlimited-archiving?view=o365-worldwide&preserve-view=true)

- [Exchange Online – Opisi usluge | Microsoft Docs](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits?redirectedfrom=MSDN#storage-limits-across-standalone-plans)

- [Nadogradnja na drugi poslovni plan | Microsoft Docs](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan?view=o365-worldwide&preserve-view=true)

