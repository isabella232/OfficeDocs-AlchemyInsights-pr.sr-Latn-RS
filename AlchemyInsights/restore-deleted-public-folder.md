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
# <a name="restore-a-deleted-public-folder"></a><span data-ttu-id="d3dab-102">Vraćanje izbrisane javne fascikle</span><span class="sxs-lookup"><span data-stu-id="d3dab-102">Restore a deleted public folder</span></span>

<span data-ttu-id="d3dab-103">**Da biste vratili izbrisane stavke iz javne fascikle:**</span><span class="sxs-lookup"><span data-stu-id="d3dab-103">**To restore deleted items from a public folder**:</span></span>

- <span data-ttu-id="d3dab-104">Pogledajte [tj. Ne možete da oporavite izbrisane stavke iz javne fascikle koja nije pošta u programu Outlook 2016.](https://aka.ms/pfrec)</span><span class="sxs-lookup"><span data-stu-id="d3dab-104">See [You can't recover deleted items from a non-mail public folder in Outlook 2016](https://aka.ms/pfrec).</span></span>
 
<span data-ttu-id="d3dab-105">**Da biste vratili izbrisanu javnu fasciklu (bilo kog tipa) u prethodno stanje:**</span><span class="sxs-lookup"><span data-stu-id="d3dab-105">**To restore a deleted public folder (of any type)**:</span></span> 

- <span data-ttu-id="d3dab-106">Koristite sledeću EXO PowerShell komandu:</span><span class="sxs-lookup"><span data-stu-id="d3dab-106">Please use following EXO PowerShell command:</span></span>

    <span data-ttu-id="d3dab-107">Sintaksa:</span><span class="sxs-lookup"><span data-stu-id="d3dab-107">Syntax:</span></span>

     `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored>`

    <span data-ttu-id="d3dab-108">Primer: Sledeća komanda će vratiti potfasciklu u prethodno stanje Potfascikla1 i postavite je u fasciklu \Parent1:</span><span class="sxs-lookup"><span data-stu-id="d3dab-108">Example: The following command will restore Subfolder1 and place it under \Parent1:</span></span>

    `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1`

<span data-ttu-id="d3dab-109">Pogledajte [vraćanje izbrisane javne fascikle](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) u prethodno stanje za više detalja.</span><span class="sxs-lookup"><span data-stu-id="d3dab-109">See [Restore a deleted public folder](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) for more details.</span></span>
