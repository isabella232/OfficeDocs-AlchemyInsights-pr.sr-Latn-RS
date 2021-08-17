---
title: Alatka za dijagnostiku usluge Windows virtuelnu radnu površinu
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003893"
- "6947"
ms.openlocfilehash: 58688e3216ba6777b1a4f76095bd39c81a2d2a8294e06b6bc61c7134f6d589f9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "54052400"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a>Alatka za dijagnostiku usluge Windows virtuelnu radnu površinu

Windows Virtuelna radna površina (WVD) nudi dijagnostičnu alatku koja omogućava adminiistantima da identifikuju greške putem jednog interfejsa. Ova alatka evidentljuje informacije vezane za dijagnostiku svaki put kada neko dodelite WVD ulogu. Svaka evidencija sadrži informacije o Ulozi VDD uključenoj u aktivnosti, porukama o grešci koje se pojavljuju tokom sesije i informacijama o zakupca i korisniku. Azure analitika evidencije može da se konfiguriše tako da uhvati evidenciju aktivnosti koju kreira dijagnostička alatka. Evo kako:

1. Kreirajte radni prostor anatike evidencije uz [Azure portal](https://go.microsoft.com/fwlink/?linkid=2129500) ili [Azure PowerShell.](https://go.microsoft.com/fwlink/?linkid=2129501)
1. [Povezivanje Windows računara na Azure Monitor](https://go.microsoft.com/fwlink/?linkid=2129913). Nabavite ID radnog prostora i primarni ključ radnog prostora. Čarobnjaku za podešavanje su potrebne ove informacije da bi ispravno konfigurisao agenta i da bi mogao da komunicira sa uslugom Azure Monitor.
1. [Push diagnostics data to your workspace](https://go.microsoft.com/fwlink/?linkid=2128284). Podatke o dijagnostici možete da gurate od WVD zakupca do ankete evidencije za radni prostor.
1. [Identifikujte i dijagnostiku](https://go.microsoft.com/fwlink/?linkid=2128338) problema koji su unutrašnji ili spoljni u odnosu na WVD.

Da biste saznali više o konfigurisanju alatke za dijagnostiku usluge za WVD, pogledajte korišćenje anatike evidencije za funkciju [dijagnostike.](https://go.microsoft.com/fwlink/?linkid=2128084)
