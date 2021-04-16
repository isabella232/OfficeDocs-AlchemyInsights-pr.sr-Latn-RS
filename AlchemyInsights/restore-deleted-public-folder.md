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
ms.openlocfilehash: d5480389c3bf50cee9fe30f7ec8d8ff28ef694ca
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/15/2021
ms.locfileid: "51809453"
---
# <a name="restore-a-deleted-public-folder"></a>Vraćanje izbrisane javne fascikle

**Da biste vratili izbrisane stavke iz javne fascikle:**

- Pogledajte [tj. Ne možete da oporavite izbrisane stavke iz javne fascikle koja nije pošta u programu Outlook 2016.](https://aka.ms/pfrec)
 
**Da biste vratili izbrisanu javnu fasciklu (bilo kog tipa) u prethodno stanje:** 

- Koristite sledeću EXO PowerShell komandu:

    Sintaksa:

     `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored>`

    Primer: Sledeća komanda će vratiti potfasciklu u prethodno stanje Potfascikla1 i postavite je u fasciklu \Parent1:

    `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1`

Pogledajte [vraćanje izbrisane javne fascikle](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) u prethodno stanje za više detalja.
