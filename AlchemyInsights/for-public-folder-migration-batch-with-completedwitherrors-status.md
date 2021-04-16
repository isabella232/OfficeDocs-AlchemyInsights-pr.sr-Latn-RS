---
title: Za paket za migraciju javne fascikle sa statusom CompletedWithErrors
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
- "3532"
ms.openlocfilehash: 9ed21bfb9069b56a4fc59b201bb3ad94c6bb6712
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/15/2021
ms.locfileid: "51812478"
---
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a>Za paket za migraciju javne fascikle sa statusom CompletedWithErrors

Koristite sledeće korake da biste dovršili paket i preskočili velike/loše stavke: 
1. Odobrite preskočene stavke u paketu za migraciju:

    `Set-MigrationBatch \<batchname> -ApproveSkippedItems` 
2. Koristite sledeću komandu da biste odobrili preskočene stavke u zahtevima za migraciju koje su "Sinhronizovane", ali nisu dovršene:

    `$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}`
3. Paket za migraciju i zahtevi treba da se nastave i završe za nekoliko minuta.

