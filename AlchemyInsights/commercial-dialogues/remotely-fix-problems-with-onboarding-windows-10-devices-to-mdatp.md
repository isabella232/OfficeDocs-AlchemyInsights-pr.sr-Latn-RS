---
title: Daljinski rešite probleme sa sistemom Windows 10 uređajima na dodatnu zaštitu pretnje u usluzi Microsoft Defender
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
ms.openlocfilehash: 5473d090f6d4680f9a62f34f943ac6cea53b2079
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/11/2021
ms.locfileid: "50750041"
---
# <a name="remotely-fix-problems-with-onboarding-windows-10-devices-to-microsoft-defender-advanced-threat-protection"></a>Daljinski rešite probleme sa sistemom Windows 10 uređajima na dodatnu zaštitu pretnje u usluzi Microsoft Defender

Ako možete da pristupite udaljenom računaru, slijedite ove korake:

1. Preuzmite dijagnostičku alatku za [Povezivanje klijenata](https://go.microsoft.com/fwlink/?linkid=2143466) .
2. Izdvajanje i pokreće Mdatpanalycer. cmd.
3. Pronađite evidenciju dijagnostike u MDATPClientAnalyzerResult fascikli, koja je ista fascikla u kojoj je preuzeta alatka analitička.
4. Da biste pronašli probleme sa povezivanjem ili postavkama Internet proxy servera, pregledajte MDATPClientAnalyzer.txt datoteku evidencije.

Da biste saznali više, pogledajte članak [problemi sa onboarnim mašinama](https://go.microsoft.com/fwlink/?linkid=2143634).
