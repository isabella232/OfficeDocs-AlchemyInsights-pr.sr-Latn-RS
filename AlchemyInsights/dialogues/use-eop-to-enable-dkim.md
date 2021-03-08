---
title: Korišćenje usluge Exchange online PowerShell za omogućavanje DKIM za određeni domen
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/23/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: 2f2b60a63b512bde794ba588852db11423e766f3
ms.sourcegitcommit: 78fe9f33438cb0c19f0dab31253b5853b73f4f47
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/05/2021
ms.locfileid: "50525242"
---
# <a name="use-exchange-online-powershell-to-enable-dkim-for-a-specific-domain"></a>Korišćenje usluge Exchange online PowerShell za omogućavanje DKIM za određeni domen

Ako ne možete da kreirate DKIM DNS zapise u centru administracije, probajte da koristite Exchange online PowerShell. 

Da biste kreirali DKIM DNS zapis pomoću usluge Exchange online PowerShell, obavite sledeće korake:

1. Otvorite Windows PowerShell kao administrator i uradite sledeće komande u opisanom redosledu:

    Neko. `$UserCredential = Get-Credential`

    -. `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    trojku. `Import-PSSession $Session -DisableNameChecking`
    
Ako imate problema sa povezivanjem sa uslugom Exchange online PowerShell, pogledajte članak [Povezivanje sa uslugom Exchange online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).

2. Kada se povežete sa Exchange online PowerShell, uradite sledeće:

    `New-DkimSigningConfig -DomainName < CustomDomain > -Enabled $true`

3. Kada se gorenavedenu komanda uspešno izvrši, uradite sledeću komandu da biste prekinuli Exchange online sesiju PowerShell sesije:

    `Remove-PSSession $Session` 



