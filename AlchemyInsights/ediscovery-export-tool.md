---
title: Alatka za izvoz e-discovery
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
- "263"
- "928"
- "1100001"
- "3100022"
ms.assetid: b16d310d-1134-4959-be68-d1c0ad463930
ms.openlocfilehash: b1100175c75fb77a499e706380305eb016cf1b2b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814602"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a>Ne možete da instalirate ili pokrenete alatku za izvoz e-discovery?

Ako ne možete da instalirate ili pokrenete alatku za izvoz e-discovery da biste preuzeli rezultate pretrage, proverite sledeće:
  
- Računar koji koristite ispunjava ove preduslove:

  - 32-bitna ili 64-bitna verzija operativnog sistema Windows 7 i novije verzije

  - Microsoft .NET Framework 4.7

  - Podržani pregledač:

  - Microsoft Edge

    Ili

  - Internet Explorer 10 i novije verzije

    Drugi pregledači, kao što su Google Chrome i Mozilla Firefox nisu podržani.

- Vaša organizacija može da se poveže sa krajnjim tačkom u programu Azure, što je **\* .blob.core.windows.net** (džoker predstavlja jedinstveni identifikator vašeg posla izvoza).

- Dodeljena vam je uloga za izvoz u Microsoft 365 centru za &amp; usaglašenost. Ova uloga se podrazumevano dodeljuje samo grupi uloga menadžera e-discovery. Pogledajte [dodela dozvola za e-discovery](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions).

Dodatne informacije potražite u [temi Izvoz rezultata pretrage sadržaja.](https://docs.microsoft.com/microsoft-365/compliance/export-search-results)

Ako izvozite više od 100K poštannih sandučića, biće potrebno da koristite sledeći PowerShell da biste preuzeli rezultate izvoza: Izvoz rezultata iz više od  [100K](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes)poštannih sandučića.