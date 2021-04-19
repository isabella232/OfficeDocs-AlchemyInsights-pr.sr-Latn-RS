---
title: Teams klijent otkazuje?
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002323"
- "4512"
ms.openlocfilehash: 20f03b075787cab85ab15d5272c0416b88ebbaee
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826285"
---
# <a name="teams-client-crashing"></a>Teams klijent otkazuje?

Ukoliko Teams klijent otkazuje, pokušajte sledeće:

- Ako koristite Teams aplikaciju za stone računare, [ uverite se da je aplikacija potpuno ažurirana](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

- Uverite se da su [svi Microsoft 365 UL adrese i opsezi](https://docs.microsoft.com/microsoftteams/connectivity-issues) adresa pristupačni.

- Prijavite se na nalog zakupca [](https://docs.microsoft.com/office365/enterprise/view-service-health) i proverite kontrolnu tablu za zdravstveno stanje usluge kako biste potvrdili da ne postoji preklovanje ili degradacija usluge.

- Deinstalacija i poništite instaliranje Teams aplikacije (veza)
    - Potražite fasciklu %appdata%\Microsoft\teams\ na računaru i izbrišite sve datoteke iz tog direktorijuma.
    - Preuzmite i [instalirajte Aplikaciju Teams](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy)i, ako je moguće, instalirajte Teams kao administrator (kliknite desnim tasterom miša na Teams instalacioni program i izaberite stavku "Pokreni kao administrator" ako je dostupno).

Ako Teams klijent i dalje pada, možete li ponovo da predstavite problem? Ako je tako:

1. Koristite zapisivač koraka da biste uhvatili korake.
    - Zatvorite SVE nepotrebne ili poverljive aplikacije.
    - Pokrenite program za snimanje koraka i ponovo predstavite problem dok ste prijavljeni sa korisničkim nalogom na koji to utiče.
    - [Prikupljajte evidencije timova koje snimaju snimljene korake repropro.](https://docs.microsoft.com/microsoftteams/log-files) **Naznaka:** Proverite da li ste zabeležili adresu za prijavljivanje upečenog korisnika.
    - Prikupite informacije o neiskladu i/ili neispravnoj kontejnneru (Windows). Pokrenite Windows PowerShell na računaru na kom je došlo do pada i pokrenite sledeće komande:

        `
        PS C:\Users\user01> cd $env:temp
        PS C:\Users\user01\AppData\Local\Temp> Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt
        PS C:\Users\user01\AppData\Local\Temp> notepad .\FaultBuckets.txt
        `
    
2. Priložite datoteku na slučaj podrške.
