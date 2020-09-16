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
# <a name="unable-to-enable-unified-auditing"></a>Nije moguće omogućiti objedinjeno nadgledanje

Kada pokušate da omogućite Objedinjeno nadgledanje za organizaciju, možete dobiti grešku sličnu sledećoj:

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

Da biste rešili ovaj problem, slijedite ove korake:

1. [Povezivanje sa uslugom Exchange online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).

2. Uradite sledeće cmdlet:

   ```
   Enable-OrganizationCustomization
   ```

3. Sačekajte 60 minuta da bi prethodna postavka stupila na snagu.

4. Uradite sledeću komandu u Exchange online PowerShell:

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

Dodatne informacije potražite u sledećim člancima:

- [Povezivanje sa Exchange online PowerShell pomoću multifaktor potvrde identiteta](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [Uključivanje ili isključivanje pretrage evidencije nadzora](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off)
