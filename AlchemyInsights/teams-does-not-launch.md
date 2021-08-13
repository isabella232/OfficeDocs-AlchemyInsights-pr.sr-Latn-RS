---
title: Teams ne pokreće se
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/4/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12673"
- "9007646"
ms.openlocfilehash: a37f980e700090da8199c703216af6f04f4aca464c21870beb3e907dd7b2d491
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "57813357"
---
# <a name="teams-doesnt-launch"></a>Teams ne pokreće se

Ako pokušate da otvorite Microsoft Teams se ne pokrene, pokušajte sledeće:

1. Idite na **%appdata%\Microsoft\Teams**.
1. Izbrišite sadržaj fascikle.
1. Ponovo pokrenite računar i pokušajte da pokrenete Teams.

Možda ćete morati ponovo da instalirate Teams. Da biste ga ponovo instalirali:

1. Deinstalujte Teams kontrolne table.
1. Potražite **%appdata%\Microsoft\Teams\Application Cache**.
1. Izbrišite sadržaj fascikle.
1. Potražite **%appdata%\Microsoft\teams\Cache**.
1. Izbrišite sadržaj fascikle.
1. Ponovo pokrenite računar, a zatim preuzmite i instalirajte Teams.

Ako na zakupcu želite da pokrenete dijagnostiku za određenog korisnika koji ne može da se prijavi, pokrenite novu pretragu sa ključnom reči **TeamsUserUnableToSignIn** i pratite odzive.