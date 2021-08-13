---
title: 2419-unable-to-enable-auditing
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
ms.openlocfilehash: 0566a8d002b1bd9e38f3184824193394e49d56494d347338f96cfcdfdb758f4c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "54007804"
---
# <a name="unable-to-enable-unified-auditing"></a>Nije moguće omogućiti nadzor u čijoj je funkciji "Nadzor"

Kada pokušate da omogućite nadzor u vašoj organizaciji, možda ćete dobiti grešku na sličan način:

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

Da biste rešili ovaj problem, pratite ove korake:

1. [Povezivanje da Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).

2. Pokrenite sledeću cmdlet cmdlet:

   ```
   Enable-OrganizationCustomization
   ```

3. Sačekajte 60 minuta da prethodna postavka stupi na snagu.

4. Pokrenite sledeću komandu u programu Exchange Online PowerShell:

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

Dodatne informacije potražite u sledećim člancima:

- [Povezivanje da Exchange Online PowerShell pomoću višestruke potvrde identiteta](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [Uključivanje ili isključivanje pretrage evidencije nadzora](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off)
