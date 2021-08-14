---
title: Primena najboljih praksi za napredne upite za potragu
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
ms.openlocfilehash: e2a22563a840cd6017afd343bad108be216738742938a48ba5ceb1010fd16098
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "53930147"
---
# <a name="apply-best-practices-for-advanced-hunting-queries"></a>Primena najboljih praksi za napredne upite za potragu

Da biste brže dobijali rezultate i izbegli vremenska perioda tokom pokretanje složenih upita, primenite ove najbolje prakse:

- Kada pokušavate nove upite, uvek koristite ograničenje da biste izbegli dobijanje izuzetno velikih skupova rezultata. Takođe, `count` koristite je za početnu procenu veličine skupa rezultata.
- Prvo koristite filtere za vreme. Idealno bi bilo da ograničite upite na sedam dana.
- Na početku upita, odmah nakon filtera vremena, dodajte filtere za koje se očekuje da uklone većinu podataka.
- Kada tražite potpune tokene, koristite `has` operator umesto `contains` .
- Pokrenite pretragu na određenoj koloni, a ne u svim kolonama.
- Prilikom pridruživanja tabelama, prvo navedite tabelu sa manje redova.
- `project` samo potrebne kolone iz tabela koje ste spojili.

Da biste saznali više, pogledajte [najbolje prakse za napredni upit za pretragu.](https://go.microsoft.com/fwlink/?linkid=2144812)
