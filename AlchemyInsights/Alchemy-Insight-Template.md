---
title: isto kao i ime datoteke je najbolje
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: b6fbaf3f2ab30888d7a8f9d6f5aeccb65b5cfd0b
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/13/2021
ms.locfileid: "58312839"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a>"Obavezno Alchemy zaglavlje H1, H2 ne funkcioniše".
Najbolje prakse i uputstva za Alchemy kreiranje:

1. **Nemojte ugnežditi Alchemy Uvidi u fascikle**– ovo će prelomiti strukturu URL adrese. Želimo da rešimo ovaj problem.
1. Datoteke u **fascikli AlchemyInsights** treba da imaju imena datoteka sa malim slovima sa crticama za razmake, ex. **_how-to-enable-litigation-hold_**.
    1. Uključite ID pravila ili ID korpe sa [portala Alchemy partner](https://alchemyportal.azurewebsites.net) u ms.custom polje. na ***ms.custom: 100021***
1. Koristite ostatak metapodataka na vrhu ove datoteke kao predložak.
1. Na [portalu "Alchemy partner"](https://alchemyportal.azurewebsites.net)možete da odte do odeljka Naslov uvida **klijenata:** i koristite ga kao početnu tačku za H1 naslov za uvid. 

**Napoma:** Alchemy Uvidi MORA da ima samo jedan H1 na vrhu ili će se prekidati u proizvodnji. H2-e se ne prikaže pa koristite **podebljanu** ili druge konvencije da biste potpisali zasebne odeljke.
1. Dalje, popunite tekst tela pomoću radne verzije materijala u Customer Insights odeljku stranice Alchemy pravilo
    1. Liste sa znakovima za nabrajanje su u redu
    1. Numerišene liste takođe
    1. **Podebljani** *i italicni* su u redu
    1. Veze uvek treba da budu "veze ka **vebu"/spoljne** ILI dubinski povezane ka elementima direktorijuma **UI**, a ne ka unutrašnjim vezama.
    1. Slike trenutno nisu zvanično podržane, ali su u toku.

A ovo je zapravo predugačak. Najbolja praksa ima oko 400 ---------------------------------

Kada sadržaj bude spreman, povucite ga do grane uživo. Zatim idite na [Alchemy portal](https://alchemyportal.azurewebsites.net) za partnere i unesite ime datoteke u polje URL adrese. 