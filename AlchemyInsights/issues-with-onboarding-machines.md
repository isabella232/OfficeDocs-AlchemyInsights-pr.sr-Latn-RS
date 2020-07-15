---
title: Problemi sa mašinama
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6023"
- "9002913"
ms.openlocfilehash: 19b516dc21472e2c80a8b9046f802b329d15e4d6
ms.sourcegitcommit: 45c2aaeee58c0be466b76c7f0cd71e796d3c8f76
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 07/15/2020
ms.locfileid: "45141659"
---
# <a name="issues-with-onboarding-machines"></a>Problemi sa mašinama

Možda imate problema sa mašinama za uslugu "MDATP". Ako možete da pristupite računaru krajnjeg korisnika, sledite ove korake:

1. Preuzmite dijagnostičku alatku [analizator veze sa klijentom](https://aka.ms/mdatpanalyzer) .
2. Izdvojite i pokrenite MDATPAnalyzer. cmd.
3. Pronađite evidenciju dijagnostike u fascikli pod nazivom Mdatpclientanalizator Zers, istu fasciklu u kojoj je preuzeta alatka za analizator.
4. Pregledajte datoteku evidencije, MDATPClientAnalyzer.txt, da biste pronašli probleme sa mogućnošću povezivanja ili proxy postavki za Internet.