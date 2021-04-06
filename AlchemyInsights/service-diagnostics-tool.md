---
title: Alatka za dijagnostiku usluge za Windows virtuelnu radnu površinu
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9004219"
- "10873"
ms.openlocfilehash: dfa59c86508c8658c880f4f3f21a002524e909d1
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/05/2021
ms.locfileid: "51595861"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a>Alatka za dijagnostiku usluge za Windows virtuelnu radnu površinu

Windows virtuelna radna površina (WVD) nudi dijagnostičnu alatku koja omogućava adminiistantima da identifikuju greške putem jednog interfejsa. Ova alatka evidentljuje informacije vezane za dijagnostiku svaki put kada neko dodelite WVD ulogu. Svaka evidencija sadrži informacije o Ulozi VDD uključenoj u aktivnosti, porukama o grešci koje se pojavljuju tokom sesije i informacijama o zakupca i korisniku. Azure analitika evidencije može da se konfiguriše tako što će pratiti ove korake za hvatanje evidencije aktivnosti koju kreira dijagnostička alatka:

1. Kreirajte radni prostor anatike evidencije uz [Azure portal](https://go.microsoft.com/fwlink/?linkid=2129500) ili [Azure PowerShell.](https://go.microsoft.com/fwlink/?linkid=2129501)

1. [Povežite Windows računare sa Azure monitorom.](https://go.microsoft.com/fwlink/?linkid=2129913) Nabavite ID radnog prostora i primarni ključ radnog prostora. Čarobnjaku za podešavanje su potrebne ove informacije da bi ispravno konfigurisao agenta i da bi mogao da komunicira sa uslugom Azure Monitor.

1. [Push diagnostics data to your workspace](https://go.microsoft.com/fwlink/?linkid=2128284). Podatke o dijagnostici možete da gurate od WVD zakupca do ankete evidencije za radni prostor.

1. [Identifikujte i dijagnostiku](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell) problema koji su unutrašnji ili spoljni u odnosu na WVD.

Da biste saznali više o konfigurisanju alatke za dijagnostiku usluge za WVD, pogledajte korišćenje anatike evidencije za funkciju dijagnostike.