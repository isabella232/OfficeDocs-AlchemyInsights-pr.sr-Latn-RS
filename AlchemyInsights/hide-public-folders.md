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
# <a name="hide-public-folders"></a>Skrivanje javnih fascikli

**Da biste sakrili celu javnu fasciklu**:

Koristite korake u [ovom](https://aka.ms/ControlPF) članku da biste sakrili celokupno stablo javne fascikle od selektivnog ili svih korisnika.

**Da biste sakrili određenu javnu fasciklu**:

1. Dodavanje dozvola za korisnike kojima je potrebno da pristupe javnoj fascikli

    `Add-PublicFolderClientPermission \test1 -User cloud1 -AccessRights owner`

2. Uklonite **podrazumevani** korisnik sa liste **dozvola** :

    `Remove-PublicFolderClientPermission \test1 -User Default`
