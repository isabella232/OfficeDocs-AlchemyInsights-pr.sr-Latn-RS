---
title: Vraćanje izbrisane javne fascikle u prethodno stanje
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3488"
ms.openlocfilehash: bb7fe248714e9a7e7f4c48913b159b5c23132192
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/15/2020
ms.locfileid: "47774545"
---
# <a name="restore-a-deleted-public-folder"></a>Vraćanje izbrisane javne fascikle u prethodno stanje

**Da biste vratili izbrisane stavke iz javne fascikle**:

- Vidite ne možete [da spasete izbrisane stavke iz javne fascikle koja nije pošta u programu Outlook 2016](https://aka.ms/pfrec).
 
**Da biste vratili izbrisane javne fascikle (bilo kog tipa)**: 

- Koristite sledeću EXO PowerShell komandu:

    Sintaksa

     `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored>`

    Primer: sledeća komanda će obnoviti Subfolder1 i postaviti je u okviru \Parent1:

    `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1`

Više detalja potražite [u članku Vraćanje izbrisane javne fascikle](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) .
