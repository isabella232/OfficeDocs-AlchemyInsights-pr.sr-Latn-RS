---
title: Razmena klasične osnovne sajta uz modernu sajt
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
ms.openlocfilehash: 10e8e4bf5e0def9a8256066e1a3c39b9923d31b0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47691193"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a>Razmena klasične osnovne sajta uz modernu sajt

Ako je okruženje podešeno pre 2019 aprila, možete da promenite osnovnu lokaciju na modernu lokaciju pomoću programa Microsoft PowerShell:

- Ako imate različitu stranicu koju želite da koristite kao osnovnu sajt, možete da je zamenite [(zamijenite) osnovnu sajt](https://docs.microsoft.com/sharepoint/modern-root-site) sa njom. 
    - Korišćenje poziva [-Spositesvp](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) za razmenu lokacije sa drugom lokacijom dok arhivirate originalnu lokaciju. Dostupno za oba sajta tima (nije povezano sa grupom) i sajt za komunikaciju. 

- Uskoro će biti predstavljene dodatne mogućnosti koje će vam omogućiti da nastavite da koristite sadržaj na sajtu, ali da konvertujete postojeću Veb na sajt za komunikaciju. 
>[!Important]
>Ove mogućnosti će se postepeno razraditi. Nastavite da proveravate centar za poruke za ispravke. 

## <a name="known-issues-with-swapping-sites"></a>Poznati problemi sa Veb lokacijama

- Ciljna lokacija može da vrati grešku "nije pronađena" (HTTP 404) na kratko vreme.
- Potrebno je ponovo popisivati sadržaj da biste ažurirali indeks pretrage. Ne postoji potreban ručni korake – ovo će biti gotovo automatski.
- Sve što zavisi od veza "statične" (kao što su sinhronizacija datoteka i OneNote datoteke) mora se ručno ispraviti.
- Ako je izvorna lokacija bila organizaciona lokacija, ažurirajte URL.Nabavite listu svih sajtova za organizacije.
- Za lokacije servera projekta možda će biti potrebno da se verifikujete da biste se uverili da su i dalje ispravno povezane.
