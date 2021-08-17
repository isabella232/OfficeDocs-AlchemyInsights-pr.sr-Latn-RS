---
title: 618 Smernice za deljenje kalendara
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
ms.openlocfilehash: 1f1bfb0273301c05f5fe5f8af5fb9039328390d16305e33897680dce1c1977e8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "54091617"
---
# <a name="policy-error-when-sharing-a-calendar"></a>Greška u smernicama prilikom deljenja kalendara

1. Uradite nešto od sledećeg, kao što je prikladno za vašu situaciju:
    - Povezivanje da Exchange Online pomoću udaljenog programa PowerShell. Dodatne informacije potražite u [Povezivanje da Exchange Online funkciju Udaljeni PowerShell.](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx)
    - Na belom serveru otvorite prozor Exchange Management Shell.
2. Odredite smernice za deljenje koje su dodeljene korisniku. Da biste to uradili, pokrenite sledeću komandu i zanemačite vraćene smernice:

    `
    Get-Mailbox User1 | fl *sharing*
    `

3. Ažuriranje smernica za deljenje za korisnika. Da biste to uradio, sledite ove korake:
    - Otvorite Exchange za administaciju.
    - Izaberite **stavku** Organizacija , a zatim kliknite dvaput na smernice koje su dodeljene korisniku u okviru **Pojedinačno deljenje.** Ovo je smernica vraćena u 2. koraku.
    - Na stranici Pravilo za deljenje izaberite nivo deljenja kalendara koji želite da dozvolite u okviru stavke **Navedite informacije koje želite da delite**; Kliknite na **dugme Sačuvaj**.

Za više informacija pogledajte: Greška "Smernice ne dozvoljavaju dodelu dozvola na ovom nivou za jednog ili više primalaca" kada korisnik pokuša da deli [kalendar.](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue)
