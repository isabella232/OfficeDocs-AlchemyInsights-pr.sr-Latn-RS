---
title: Vraćanje izbrisane javne fascikle
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3488"
ms.openlocfilehash: 6df196fc0bde37c962e3aa84dd602ee414dad3d329addfd16cb6e3dcc40fc2ae
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "53943389"
---
# <a name="restore-a-deleted-public-folder"></a>Vraćanje izbrisane javne fascikle

**Da biste vratili izbrisane stavke iz javne fascikle:**

- Pogledajte [tj. Nije moguće oporaviti izbrisane stavke iz javne fascikle koja nije pošta u programu Outlook 2016.](https://aka.ms/pfrec)
 
**Da biste vratili izbrisanu javnu fasciklu (bilo kog tipa) u prethodno stanje:** 

- Koristite sledeću EXO PowerShell komandu:

    Sintaksa:

     `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored>`

    Primer: Sledeća komanda će vratiti potfasciklu u prethodno stanje Potfascikla1 i postavite je u fasciklu \Parent1:

    `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1`

Pogledajte [vraćanje izbrisane javne fascikle](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) u prethodno stanje za više detalja.
