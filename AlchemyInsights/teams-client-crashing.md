---
title: Teams klijent pada
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
ms.openlocfilehash: bef16351b55ac4765539d66ab86a71183f66f0dd
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/13/2021
ms.locfileid: "58321639"
---
# <a name="teams-client-crashing"></a>Teams klijent pada

Ukoliko Teams klijent otkazuje, pokušajte sledeće:

- Ako koristite Teams aplikaciju za stone računare, [ uverite se da je aplikacija potpuno ažurirana](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).

- Uverite se da [su Microsoft 365 ULS i opsezi](https://docs.microsoft.com/microsoftteams/connectivity-issues) adresa.

- Prijavite se na nalog zakupca [](https://docs.microsoft.com/office365/enterprise/view-service-health) i proverite kontrolnu tablu za zdravstveno stanje usluge kako biste potvrdili da ne postoji preklonje ili degradacija usluge.

- Deinstalujte i ponovo instalirajte aplikaciju Teams aplikaciju
    - Potražite fasciklu %appdata%\Microsoft\Teams\ na računaru i izbrišite sve datoteke iz tog direktorijuma.
    - Preuzmite i instalirajte [Teams](https://www.microsoft.com/microsoft-teams/download-app)aplikaciju i, ako je moguće, instalirajte Teams kao administrator (kliknite desnim tasterom miša na instalacioni program za Teams i izaberite stavku Pokreni kao **administrator** ako je dostupno).

Ako Teams klijent i dalje pada, pokušajte ponovo da predstavite problem. Ako možete da:

1. Koristite zapisivač koraka da biste uhvatili korake.
    - Zatvorite SVE nepotrebne ili poverljive aplikacije.
    - Pokrenite program za snimanje koraka i ponovo predstavite problem dok ste prijavljeni sa korisničkim nalogom na koji to utiče.
    - [Prikupljajte evidencije timova koje snimaju snimljene korake repropro.](https://docs.microsoft.com/microsoftteams/log-files) 
    
    **Naznaka:** Proverite da li ste zabeležili adresu za prijavljivanje upečenog korisnika.
    - Prikupite informacije o neis kvaru i/ili neispravnu kontejner (ili Windows). Pokrenite Windows PowerShell na računaru na kojem je došlo do pada i pokrenite sledeće komande (nakon svake komande pritisnite taster Enter):

    `cd $env:temp` `Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt`
    `notepad .\FaultBuckets.txt`
    
2. Kada se tekstualna datoteka generiše i pojavi na ekranu, sačuvajte je i priložite zahtevu za uslugom. 
