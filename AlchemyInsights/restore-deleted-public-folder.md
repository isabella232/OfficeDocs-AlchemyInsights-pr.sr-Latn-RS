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
# <a name="restore-a-deleted-public-folder"></a><span data-ttu-id="48251-102">Vraćanje izbrisane javne fascikle u prethodno stanje</span><span class="sxs-lookup"><span data-stu-id="48251-102">Restore a deleted public folder</span></span>

<span data-ttu-id="48251-103">**Da biste vratili izbrisane stavke iz javne fascikle**:</span><span class="sxs-lookup"><span data-stu-id="48251-103">**To restore deleted items from a public folder**:</span></span>

- <span data-ttu-id="48251-104">Vidite ne možete [da spasete izbrisane stavke iz javne fascikle koja nije pošta u programu Outlook 2016](https://aka.ms/pfrec).</span><span class="sxs-lookup"><span data-stu-id="48251-104">See [You can't recover deleted items from a non-mail public folder in Outlook 2016](https://aka.ms/pfrec).</span></span>
 
<span data-ttu-id="48251-105">**Da biste vratili izbrisane javne fascikle (bilo kog tipa)**:</span><span class="sxs-lookup"><span data-stu-id="48251-105">**To restore a deleted public folder (of any type)**:</span></span> 

- <span data-ttu-id="48251-106">Koristite sledeću EXO PowerShell komandu:</span><span class="sxs-lookup"><span data-stu-id="48251-106">Please use following EXO PowerShell command:</span></span>

    <span data-ttu-id="48251-107">Sintaksa</span><span class="sxs-lookup"><span data-stu-id="48251-107">Syntax:</span></span>

     `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored>`

    <span data-ttu-id="48251-108">Primer: sledeća komanda će obnoviti Subfolder1 i postaviti je u okviru \Parent1:</span><span class="sxs-lookup"><span data-stu-id="48251-108">Example: The following command will restore Subfolder1 and place it under \Parent1:</span></span>

    `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1`

<span data-ttu-id="48251-109">Više detalja potražite [u članku Vraćanje izbrisane javne fascikle](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) .</span><span class="sxs-lookup"><span data-stu-id="48251-109">See [Restore a deleted public folder](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) for more details.</span></span>
