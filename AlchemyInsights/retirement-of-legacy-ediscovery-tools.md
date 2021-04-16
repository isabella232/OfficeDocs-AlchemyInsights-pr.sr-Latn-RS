---
title: Retirement of Legacy eDiscovery Tools
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
- "9001487"
- "3523"
ms.openlocfilehash: 986c78f20e7b8c303c302913d63d817a56ce2896
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/15/2021
ms.locfileid: "51798563"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a>Retirement of Legacy eDiscovery Tools

Kao rezultat nove i poboljšane funkcionalnosti e-discovery u Microsoft 365 centru za usaglašenost, sledeće zakupne alatke za e-discovery i komande će biti poništene u sledećim mesecima:

- [Čuvanje čuvanja e-čuvanja](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) na mestu u Exchange centru adminitre. [](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds)

- Exchange Online PowerShell cmdlet In-Place e-discovery i čuvanje In-Place čuvanja podataka. (Ove cmdletlet menije su kolektivno identifikovane kao *-MailboxSearch cmdlets.) To uključuje sledeće cmdlet mišove:

    - [New-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [Start-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [Stop-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [Set-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- Cmdlet [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) u programu Exchange Online PowerShell.
- Sledeće operacije u API-u Exchange veb usluga:
    - [GetSearchableMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [SetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [GetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [Advanced eDiscovery v1.0](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

**Vremenska linija za penzionje:**
- **1. jul 2020.** Više ne možete da kreirate nove pretrage i zadrške, ali možete da pokrećete, uređujete i brišete postojeće pretrage na sopstveni rizik. Microsoft podrška više ne podržava čuvanje In-Place e-& u EAC-u.
    
- **1. oktobar 2020.** In-Place funkcionalnost & čuvanja čuvanja u EAC-u biće postavljena u režim samo za čitanje, tako da možete da uklonite samo postojeće pretrage i zadrške.

**Dodatne informacije potražite u:**

 - [Migrirane zakasnele pretrage i zadrške u Microsoft 365 centru za usaglašenost](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [Retirement of legacy eDiscovery tools](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [FaQs about In-Place e-discovery and In-Place Holds](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



