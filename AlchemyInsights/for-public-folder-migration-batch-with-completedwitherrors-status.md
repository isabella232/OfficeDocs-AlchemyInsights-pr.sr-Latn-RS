---
title: Za grupnu obradu za migraciju javnih fascikli sa ispravnim greškama
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
- "3532"
ms.openlocfilehash: cbf5237fdb5c660057465e67702e35f68e545ddb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47744127"
---
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a>Za grupnu obradu za migraciju javnih fascikli sa ispravnim greškama

Koristite sledeće korake da biste dovršili grupnu obradu, preskakanje velikih/pogrešnih stavki: 
1. Odobravanje preskočenih stavki o migraciji:

    `Set-MigrationBatch \<batchname> -ApproveSkippedItems` 
2. Koristite sledeću komandu da biste odobrili preskočene stavke u zahtevima za migraciju koji su "sinhronizovani", ali nisu dovršeni:

    `$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}`
3. Grupa i zahtevi za migraciju treba da se nastave i završe za nekoliko minuta.

