---
title: Daljinsko rešavanje problema sa Windows 10 uređaja u Microsoft zaštitnik Napredna zaštita od pretnji
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
ms.openlocfilehash: 44969436c99b182cb4202fa60e2deb7d6ea3f460e48ee4649de1cfb646970f34
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "54034048"
---
# <a name="remotely-fix-problems-with-onboarding-windows-10-devices-to-microsoft-defender-advanced-threat-protection"></a>Daljinsko rešavanje problema sa Windows 10 uređaja u Microsoft zaštitnik Napredna zaštita od pretnji

Ako možete da pristupite udaljenom računaru, sledite ove korake:

1. Preuzmite [dijagnostiku analizatora klijentskih](https://go.microsoft.com/fwlink/?linkid=2143466) povezivanja.
2. Izdvajanje i pokretanje MDATPAnalyzer.cmd.
3. Pronađite evidenciju dijagnostike u fascikli MDATPClientAnalyzerResult, koja je ista fascikla u kojoj je preuzeta alatka analyzer.
4. Da biste pronašli probleme sa povezivanjem ili postavkama internet proxy servera, pregledajte datoteku evidencije MDATPClientAnalyzer.txt.

Da biste saznali više, pogledajte [problem sa mašinama za ulaženje u avion](https://go.microsoft.com/fwlink/?linkid=2143634).
