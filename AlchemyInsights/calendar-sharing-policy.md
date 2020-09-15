---
title: 618 smernice za deljenje kalendara
ms.author: chrisda
author: chrisda
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "618"
- "899"
- "3800014"
ms.assetid: bc3db17b-87f8-4e50-b3ee-8b105b70d67a
ms.openlocfilehash: d2511183d068330cdcfb4e08b08df4f18625c822
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47684244"
---
# <a name="policy-error-when-sharing-a-calendar"></a>Greška u smernicama prilikom deljenja kalendara

1. Uradite nešto od sledećeg, u skladu sa situacijom:
    - Povežite se sa uslugom Exchange online pomoću udaljenog PowerShell. Više informacija potražite u članku [Povezivanje sa uslugom Exchange online pomoću udaljenog PowerShell](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).
    - Na lokalnom serveru otvorite karticu upravljanje Exchange serverom.
2. Odredite smernice za deljenje koje su dodeljene korisniku. Da biste to uradili, izvršite sledeću komandu i napomena vraćene smernice:

    `
    Get-Mailbox User1 | fl *sharing*
    `

3. Ažurirajte smernice za deljenje za korisnika. Da biste to uradili, pratite ove korake:
    - Otvorite Exchange centar administracije.
    - Izaberite stavku **organizacija**, a zatim kliknite dvaput na smernice koje su dodeljene korisniku u okviru **pojedinačno deljenje**. Ovo su smernice vraćene u 2.
    - Na stranici pravilo za deljenje izaberite nivo deljenja kalendara koji želite da omogućite u okviru **navedite koje informacije želite da delite**; Kliknite na dugme **Sačuvaj**.

Više informacija potražite u članku: ["smernice ne dozvole dodeljivanje dozvola na ovom nivou jednoj ili više primalaca" kada korisnik pokuša da deli kalendar](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue).
