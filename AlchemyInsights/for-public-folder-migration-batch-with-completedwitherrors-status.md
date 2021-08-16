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
ms.openlocfilehash: 78ceac80626159e72af5f9ac963365c5c057a4ef0de2b3dc7e4cde5e5cc155e5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "54068178"
---
# <a name="for-public-folder-migration-batch-with-completedwitherrors-status"></a>Za paket za migraciju javne fascikle sa statusom CompletedWithErrors

Koristite sledeće korake da biste dovršili paket i preskočili velike/loše stavke: 
1. Odobrite preskočene stavke u paketu za migraciju:

    `Set-MigrationBatch \<batchname> -ApproveSkippedItems` 
2. Koristite sledeću komandu da biste odobrili preskočene stavke u zahtevima za migraciju koje su "Sinhronizovane", ali nisu dovršene:

    `$pf=Get-PublicFolderMailboxMigrationRequest | Get-PublicFolderMailboxMigrationRequestStatistics -IncludeReport; ForEach ($i in $pf) {if ($i.LargeItemsEncountered -gt 0 -or $i.BadItemsEncountered -gt 0) {Set-PublicFolderMailboxMigrationRequest $i.Identity.IdentifyingGuid -SkippedItemApprovalTime $([DateTime]::UtcNow)}}`
3. Paket za migraciju i zahtevi treba da se nastave i završe za nekoliko minuta.

