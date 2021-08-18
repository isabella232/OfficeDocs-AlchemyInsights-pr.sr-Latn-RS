---
title: Zamena klasičnog osnovnog sajta sa modernim sajtom
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: e8501414498bf1937e98abaca32987e3276bb54e
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/13/2021
ms.locfileid: "58316154"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a>Zamena klasičnog osnovnog sajta sa modernim sajtom

Ako je okruženje podešeno pre aprila 2019, osnovnu lokaciju možete da promenite u modernu lokaciju pomoću programa Microsoft PowerShell:

- Ako imate drugi sajt koji želite da koristite kao osnovni sajt, možete da zamenite [osnovni](https://docs.microsoft.com/sharepoint/modern-root-site) sajt sa njim. 
    - Koristite [invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) da biste zamenili lokaciju lokacije sa drugim sajtom prilikom arhiviranje originalnog sajta. Dostupno za sajt tima (nije povezan sa grupom) i sajtu za komunikaciju. 

- Dodatne mogućnosti će se uskoro uvesti koje će vam omogućiti da nastavite da koristite sadržaj na lokaciji, ali da konvertujete postojeći sajt u sajt za komunikaciju. 

**Važno:** Ove mogućnosti će se postepeno izlaziti. Nastavite da biste proverili da li u centru za poruke postoje ispravke. 

## <a name="known-issues-with-swapping-sites"></a>Poznati problemi sa zamenom sajtova

- Ciljni sajt može dati grešku "nije pronađeno" (HTTP 404) tokom kratkog vremenskog perioda.
- Sadržaj treba ponovo da se pretražuje da bi se ažurirao indeks za pretraživanje. Ne postoji ručni korak – ovo će se uraditi automatski.
- Sve što zavisi od "statičnih" veza (kao što su sinhronizacija datoteka i OneNote datoteke) moraće ručno da se ispravi.
- Ako je izvorna lokacija bila sajt organizacionih vesti, ažurirajte URL. Nabavite listu svih sajtova organizacionih vesti.
- Project Možda će biti potrebno proveriti valjanost lokacija servera da biste se uverili da su i dalje ispravno povezane.
