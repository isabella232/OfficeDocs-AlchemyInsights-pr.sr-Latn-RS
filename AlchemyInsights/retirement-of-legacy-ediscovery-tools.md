---
title: Penzija nasleđenih alatki za eDiscovery
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001487"
- "3523"
ms.openlocfilehash: 94cd2127240be5faacd397ba6255fdb16e364308
ms.sourcegitcommit: d4fc2a03af69e28e96075812d040fdd34d2e23f0
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/26/2020
ms.locfileid: "46902634"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a>Penzija nasleđenih alatki za eDiscovery

Kao rezultat nove i poboljšane funkcionalne funkcionalnosti u Microsoft 365 centru za usaglašenost, sledeće zastarele alatke za eDiscovery i zapovesti će se vratiti u narednih nekoliko meseci:

- U [mestu eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) i [na](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) mestu se nalazi u Exchange centru administracije.

- Exchange online PowerShell cmdlet komande koji podržavaju funkcije ediscovery i na mestu će ga čuvati. (Ovi cmdlet zapisi kolektivno su identifikovani kao *-mailboxsearch cmdlet komande.) To uključuje sledeće cmdlet sledeće:

    - [Novo-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [Start-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [Stop-pošta Boxsearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [Scenofor-MailboxSearch](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- [Pretraga – poštansko sanduče](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) cmdlet usluge Exchange online PowerShell.
- Sledeće operacije u usluzi Exchange Veb Services:
    - [Getsearchablemailbox](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [Setholdone sandučići](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [Getholdone sandučići](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [Napredno eDiscovery v 1.0](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

**Vremenska osa za penziju**:
- **1. jul, 2020** Više ne možete da kreirate nove pretrage i zadržavanje, ali možete da pokrećete, uređujete i brišete postojeće pretrage po sopstvenom riziku. Microsoft Support više ne podržava na mjestu eDiscovery & čuva u EAC-u.
    
- **1 oktobar, 2020** Funkcija "eDiscovery &" u EAC-u biće postavljena u režimu samo za čitanje, tako da možete da uklonite samo postojeće pretrage i zadrške.

**Više informacija potražite u članku**:

 - [Migriranje zastarelih eDiscovery pretraga i držanje u Microsoft 365 centru za usaglašenost](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [Penzija nasleđenih alatki za eDiscovery](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [Najčešća pitanja o otkrivanju na mestu koje se nalazi na sajtu i održavaju se na mestu](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



