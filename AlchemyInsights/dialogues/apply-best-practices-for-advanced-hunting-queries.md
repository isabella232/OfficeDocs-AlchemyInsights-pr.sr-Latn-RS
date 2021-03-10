---
title: Primenjivanje najboljih praksi za napredne lovačke upite
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: cd13e2e8801db3df91140ce371813d900d72e38b
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/09/2021
ms.locfileid: "50696085"
---
# <a name="apply-best-practices-for-advanced-hunting-queries"></a>Primenjivanje najboljih praksi za napredne lovačke upite

Da biste brže pokrenuli rezultate i izbegli vremenska ograničenja prilikom pokretanja složenih upita, primene ove najbolje prakse:

- Prilikom pokušaja novih upita, uvek koristite limit da biste izbegli izuzetno velike skupove ishoda. Pored toga, koristite `count` ga da biste napravili inicijalnu procenu veličine skupa ishoda.
- Najpre koristite vremenske filtere. Idealno, ograničite upite na sedam dana.
- Na početku upita, odmah posle filtera vremena, dodajte filtere za koje se očekuje da će ukloniti većinu podataka.
- Kada tražite pune simbole, koristite `has` operator umesto `contains` .
- Pokrećete pretragu u određenoj koloni, a ne u svim kolonama.
- Prilikom pridruživanja tabelama, prvo navedite tabelu sa manje redova.
- `project` Samo neophodne kolone iz tabela kojima ste se pridružili.

Da biste saznali više, pogledajte članak [Napredni osnovni načini za lov Query](https://go.microsoft.com/fwlink/?linkid=2144812).
