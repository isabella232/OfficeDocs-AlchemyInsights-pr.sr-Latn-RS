---
title: Postavite ClientAccessServerEnabled na True
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: b134c952e3cc5305d8f3e6f44031e7f33d7938b67ff122c46cb74bbd33cbf59e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "53994879"
---
# <a name="set-clientaccessserverenabled-to-true"></a>Postavite ClientAccessServerEnabled na True

Ako ne možete da otvorite šifrovanu e-poruku i umesto toga vidite **rpmsg** prilog, izvršite sledeće korake:

1. Povezivanje da Exchange Online PowerShell.

> [!NOTE]
> Da biste se povezali Exchange Online programu PowerShell, morate da se prijavite pomoću globalnog ili Exchange naloga za administratovanje.

   a. Otvorite Windows PowerShell, a zatim pokrenite sledeću komandu:`$UserCredential = Get-Credential`
b. U dijalog Windows PowerShell Zahtev za **akredi** nije moguće uneti poslovni ili školski nalog i lozinku, c. Kliknite na dugme **U redu**. 

2. Pokrenite sledeću komandu da biste kreirali novu sesiju:

    `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    a. Pokrenite sledeću komandu:
    
    `Import-PSSession $Session -DisableNameChecking`

3. Komanda `Get-IRMConfiguration` "Pokreni".

4. Proverite **postavku ClientAccessServerEnabled.** 

    a. Ako **je postavka ClientAccessServerEnabled** postavljena na **False,** pokrenite sledeću cmdlet radnju: `Set-IRMConfiguration -ClientAccessServerEnabled $True`

> [!TIP]
> Uvek zatvorite PowerShell sesiju uz sledeću komandu: `Remove-PSSession $Session`

Dodatne informacije potražite u [Exchange Online PowerShell.](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell)

