---
title: Skrivanje javnih fascikli
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/18/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "8417"
ms.openlocfilehash: 70179296e9c1bb7391535f55796bc5af80b825f8
ms.sourcegitcommit: a019bd8b0244914edb59e124bc6538cdc5c158f9
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 02/18/2021
ms.locfileid: "50315438"
---
# <a name="hide-public-folders"></a><span data-ttu-id="83d83-102">Skrivanje javnih fascikli</span><span class="sxs-lookup"><span data-stu-id="83d83-102">Hide public folders</span></span>

<span data-ttu-id="83d83-103">**Da biste sakrili celu javnu fasciklu**:</span><span class="sxs-lookup"><span data-stu-id="83d83-103">**To hide entire public folder tree**:</span></span>

<span data-ttu-id="83d83-104">Koristite korake u [ovom](https://aka.ms/ControlPF) članku da biste sakrili celokupno stablo javne fascikle od selektivnog ili svih korisnika.</span><span class="sxs-lookup"><span data-stu-id="83d83-104">Use the steps in [this](https://aka.ms/ControlPF) article to hide entire public folder tree from selective or all users.</span></span>

<span data-ttu-id="83d83-105">**Da biste sakrili određenu javnu fasciklu**:</span><span class="sxs-lookup"><span data-stu-id="83d83-105">**To hide a specific public folder**:</span></span>

1. <span data-ttu-id="83d83-106">Dodavanje dozvola za korisnike kojima je potrebno da pristupe javnoj fascikli</span><span class="sxs-lookup"><span data-stu-id="83d83-106">Add permissions for users who need to access the public folder</span></span>

    `Add-PublicFolderClientPermission \test1 -User cloud1 -AccessRights owner`

2. <span data-ttu-id="83d83-107">Uklonite **podrazumevani** korisnik sa liste **dozvola** :</span><span class="sxs-lookup"><span data-stu-id="83d83-107">Remove the user **Default** from the **permission** list:</span></span>

    `Remove-PublicFolderClientPermission \test1 -User Default`
