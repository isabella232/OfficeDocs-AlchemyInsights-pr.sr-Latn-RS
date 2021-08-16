---
title: Korišćenje Exchange Online PowerShell za omogućavanje usluge DKIM za određeni domen
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
ms.openlocfilehash: ba627c6da96624914b858aa09d6eff9de709134c2c986fe363845c5ab2b66434
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "54070328"
---
# <a name="use-exchange-online-powershell-to-enable-dkim-for-a-specific-domain"></a>Korišćenje Exchange Online PowerShell za omogućavanje usluge DKIM za određeni domen

Ako ne možete da kreirate DKIM DNS zapise u centru aktivnosti, pokušajte da koristite Exchange Online PowerShell. 

Da biste kreirali DKIM DNS zapis pomoću Exchange Online PowerShell, izvršite sledeće korake:

1. Otvorite Windows PowerShell kao administrator i pokrenite sledeće komande opisanom nizom:

    a. `$UserCredential = Get-Credential`

    b. `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    c. `Import-PSSession $Session -DisableNameChecking`
    
Ako imate problema pri povezivanju sa Exchange Online PowerShell, pogledajte Povezivanje [se Exchange Online PowerShell.](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell)

2. Kada se povežete sa programom Exchange Online PowerShell, pokrenite sledeću komandu:

    `New-DkimSigningConfig -DomainName < CustomDomain > -Enabled $true`

3. Kada se gorenavedena komanda uspešno izvrši, pokrenite sledeću komandu da biste obustavljali Exchange Online PowerShell sesije:

    `Remove-PSSession $Session` 



