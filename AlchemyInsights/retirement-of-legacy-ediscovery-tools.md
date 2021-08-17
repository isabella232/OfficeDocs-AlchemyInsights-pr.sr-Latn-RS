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
ms.openlocfilehash: 2e7f898ac1a9e9469f633192be18e2a3a362023c83c9e510593196b5a4a0daf5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "54074688"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a>Retirement of Legacy eDiscovery Tools

Kao rezultat nove i poboljšane funkcionalnosti e Microsoft 365 centra za usaglašenost, sledeće zakupne alatke za e-discovery i komande će biti poništene u sledećim mesecima:

- [Čuvanje čuvanja e-čuvanja](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) na mestu Exchange centra za adminitre. [](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds)

- The Exchange Online PowerShell cmdletlets that support In-Place e-discovery and In-Place Holds. (Ove cmdletlet menije su kolektivno identifikovane kao *-MailboxSearch cmdlets.) To uključuje sledeće cmdlet mišove:

    - [New-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [Start-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [Stop-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [Set-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- Cmdlet [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) u programu Exchange Online PowerShell.
- Sledeće operacije u API-Exchange veb usluga:
    - [GetSearchableMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [SetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [GetHoldOnMailboxes](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [Advanced eDiscovery v1.0](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

**Vremenska linija za penzionje:**
- **1. jul 2020.** Više ne možete da kreirate nove pretrage i zadrške, ali možete da pokrećete, uređujete i brišete postojeće pretrage na sopstveni rizik. Microsoft podrška više ne podržava čuvanje In-Place e-& u EAC-u.
    
- **1. oktobar 2020.** In-Place funkcionalnost & čuvanja čuvanja u EAC-u biće postavljena u režim samo za čitanje, tako da možete da uklonite samo postojeće pretrage i zadrške.

**Dodatne informacije potražite u:**

 - [Migrirane zakasnele pretrage i zadrške u Microsoft 365 centar za usaglašenost](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [Retirement of legacy eDiscovery tools](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [FaQs about In-Place e-discovery and In-Place Holds](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



