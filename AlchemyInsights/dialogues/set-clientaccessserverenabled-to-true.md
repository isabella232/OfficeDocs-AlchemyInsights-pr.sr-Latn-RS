---
title: Podesi ClientAccessServerEnabled na TRUE
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
ms.openlocfilehash: 2adf35662797e9e9e354ddd0c513f5ce2463d07c
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/05/2021
ms.locfileid: "50525963"
---
# <a name="set-clientaccessserverenabled-to-true"></a>Podesi ClientAccessServerEnabled na TRUE

Ako ne možete da otvorite šifrovanu e-poruku i da vidite prilog **rpmsg** , izvršite sledeće korake:

1. Povezivanje sa uslugom Exchange online PowerShell.

> [!NOTE]
> Da biste se povezali sa uslugom Exchange online PowerShell, morate da se prijavite pomoću globalnog administratora ili Exchange naloga administracije.

   Neko. Otvorite Windows PowerShell, a zatim uradite sledeće: `$UserCredential = Get-Credential`
-. U dijalogu **zahtev za akreditiva Windows PowerShell** unesite poslovni ili školski nalog i lozinku, c. Kliknite na dugme **U redu**. 

2. Uradite sledeće komande da biste kreirali novu sesiju:

    `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    Neko. Uradite sledeće:
    
    `Import-PSSession $Session -DisableNameChecking`

3. `Get-IRMConfiguration`Komanda "pokrene".

4. Potvrdite postavku **Clientaccessserverenabled** . 

    Neko. Ako je postavka **Clientaccessserverenabled** postavljena na **vrednost FALSE**, uradite sledeće cmdlet lokacije: `Set-IRMConfiguration -ClientAccessServerEnabled $True`

> [!TIP]
> Uvek zatvorite sesiju PowerShell sa sledećim komandama: `Remove-PSSession $Session`

Više informacija potražite u članku [Exchange online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).

