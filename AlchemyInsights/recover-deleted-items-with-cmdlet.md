---
title: Oporavak izbrisanih stavki uz cmdlet
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1800008"
- "5718"
ms.openlocfilehash: d8f2a50f39d7bcd321692ab093e2efa6613e9814
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/15/2021
ms.locfileid: "51835825"
---
# <a name="recover-deleted-items-with-cmdlet"></a><span data-ttu-id="226d6-102">Oporavak izbrisanih stavki uz cmdlet</span><span class="sxs-lookup"><span data-stu-id="226d6-102">Recover deleted items with cmdlet</span></span>

- <span data-ttu-id="226d6-103">Koristite cmdlet [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) da biste prikazali izbrisane stavke u poštanskim sandučićima.</span><span class="sxs-lookup"><span data-stu-id="226d6-103">Use the [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) cmdlet to view deleted items in mailboxes.</span></span> <span data-ttu-id="226d6-104">Kada pronađete izbrisane stavke, koristite cmdlet [Restore-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/Restore-RecoverableItems?view=exchange-ps) da biste ih vratili.</span><span class="sxs-lookup"><span data-stu-id="226d6-104">After you find the deleted items, you use the [Restore-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/Restore-RecoverableItems?view=exchange-ps) cmdlet to restore them.</span></span>

- <span data-ttu-id="226d6-105">Pogledajte sve detalje u [temi Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="226d6-105">See full details in [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps).</span></span>

- <span data-ttu-id="226d6-106">Da biste mogli da pokrenete ovu cmdlet, mora da vam se dodelite uloga uvoza i izvoza poštanskog sandučeta.</span><span class="sxs-lookup"><span data-stu-id="226d6-106">You need to be assigned the Mailbox Import Export role before you can run this cmdlet.</span></span> <span data-ttu-id="226d6-107">Više informacija [potražite u temi Get-RecoverableItems.](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps)</span><span class="sxs-lookup"><span data-stu-id="226d6-107">Please see [Get-RecoverableItems](https://docs.microsoft.com/powershell/module/exchange/get-recoverableitems?view=exchange-ps) for more information.</span></span>
