---
title: Alatka za izvoz e-otkrivanja
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
- "263"
- "928"
- "1100001"
- "3100022"
ms.assetid: b16d310d-1134-4959-be68-d1c0ad463930
ms.openlocfilehash: 67e59182a5053111a08f5fb2be814931a1aa815d
ms.sourcegitcommit: fbe6925797cab0b38172386f1b059dc122e452a4
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/25/2020
ms.locfileid: "48277954"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a>Ne možete da instalirate ili pokrećete alatku za izvoz eDiscovery?

Ako ne možete da instalirate ili izvršite alatku za izvoz eDiscovery za preuzimanje rezultata pretrage, potvrdite sledeće stvari:
  
- Računar koji koristite ispunjava ove unapred zahteve:

  - 32-ili 64-bitne verzije operativnog sistema Windows 7 i novije verzije

  - Microsoft .NET Framework 4.7

  - Podržani pregledač:

  - Microsoft Edge

    Jer

  - Internet Explorer 10 i novije verzije

    Drugi pregledači, na primer Google Chrome i Mozilla Firefox nisu podržani.

- Vaša organizacija može da se poveže sa krajnjim tačkom u Azure, što je ** \* . BLOB.Core.Windows.net** (džoker predstavlja Jedinstveni identifikator za posao izvoza).

- Dodeljena vam je uloga izvoza u Microsoft 365 bezbednosnom &amp; centru za usaglašenost. Ova uloga se podrazumevano dodeljuje samo grupi uloga programa eDiscovery. Pogledajte [dodelu dozvola za eDiscovery](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions).

Više informacija potražite u članku [izvoz rezultata pretrage sadržaja](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).

Ako izvozite više od 100K poštanskih sandučića, moraćete da koristite sledeće PowerShell za preuzimanje rezultata izvoza:  [izvoz rezultata iz više od 100k poštanskih sandučića](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).