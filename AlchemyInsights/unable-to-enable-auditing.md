---
title: 2419-revizija nije moguće-omogućavanje-omogućavanje-revizija
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 2419
ms.assetid: ''
ms.openlocfilehash: 81fd8e33feb2f2b10b04cc7cdc746a8603aa366b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/15/2020
ms.locfileid: "47767613"
---
# <a name="unable-to-enable-unified-auditing"></a><span data-ttu-id="f87c2-102">Nije moguće omogućiti objedinjeno nadgledanje</span><span class="sxs-lookup"><span data-stu-id="f87c2-102">Unable to enable unified auditing</span></span>

<span data-ttu-id="f87c2-103">Kada pokušate da omogućite Objedinjeno nadgledanje za organizaciju, možete dobiti grešku sličnu sledećoj:</span><span class="sxs-lookup"><span data-stu-id="f87c2-103">When you try to enable unified auditing for your organization, you may receive an error similar the following:</span></span>

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

<span data-ttu-id="f87c2-104">Da biste rešili ovaj problem, slijedite ove korake:</span><span class="sxs-lookup"><span data-stu-id="f87c2-104">To resolve this issue, follow these steps:</span></span>

1. <span data-ttu-id="f87c2-105">[Povezivanje sa uslugom Exchange online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).</span><span class="sxs-lookup"><span data-stu-id="f87c2-105">[Connect to Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).</span></span>

2. <span data-ttu-id="f87c2-106">Uradite sledeće cmdlet:</span><span class="sxs-lookup"><span data-stu-id="f87c2-106">Run the following cmdlet:</span></span>

   ```
   Enable-OrganizationCustomization
   ```

3. <span data-ttu-id="f87c2-107">Sačekajte 60 minuta da bi prethodna postavka stupila na snagu.</span><span class="sxs-lookup"><span data-stu-id="f87c2-107">Wait for 60 minutes for the previous setting to take effect.</span></span>

4. <span data-ttu-id="f87c2-108">Uradite sledeću komandu u Exchange online PowerShell:</span><span class="sxs-lookup"><span data-stu-id="f87c2-108">Run the following command in Exchange Online PowerShell:</span></span>

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

<span data-ttu-id="f87c2-109">Dodatne informacije potražite u sledećim člancima:</span><span class="sxs-lookup"><span data-stu-id="f87c2-109">For additional information, see the following articles:</span></span>

- [<span data-ttu-id="f87c2-110">Povezivanje sa Exchange online PowerShell pomoću multifaktor potvrde identiteta</span><span class="sxs-lookup"><span data-stu-id="f87c2-110">Connect to Exchange Online PowerShell using multi-factor authentication</span></span>](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [<span data-ttu-id="f87c2-111">Uključivanje ili isključivanje pretrage evidencije nadzora</span><span class="sxs-lookup"><span data-stu-id="f87c2-111">Turn audit log search on or off</span></span>](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off)
