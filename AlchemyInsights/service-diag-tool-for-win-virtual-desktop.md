---
title: Alatka za dijagnostiku usluge za Windows virtuelnu radnu površinu
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
ms.openlocfilehash: c2e6f7fbcddc6721425840e87202a165cdb22664
ms.sourcegitcommit: 87bf574162e536003164ff9af50005c5a7dce601
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 12/14/2020
ms.locfileid: "49680230"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a>Alatka za dijagnostiku usluge za Windows virtuelnu radnu površinu

Windows virtuelna radna površina (WVD) nudi dijagnostičku alatku koja omogućava administratori da identifikuju greške kroz jedan interfejs. Ova alatka evidentira informacije vezane za dijagnostiku kad god WVD koristi neko ko mu je dodeljen. Svaka evidencija sadrži informacije o WVD ulozi koja je uključena u aktivnost, poruke o greškama koje se pojavljuju tokom sesije i informacije o zakupcu i korisniku. Azure evidencija Analitika može da se konfiguriše za hvatanje evidencije aktivnosti kreirane pomoću alatke za dijagnostiku. Evo kako:

1. Kreirajte radni prostor evidencije evidentiranja pomoću [Azure portala](https://go.microsoft.com/fwlink/?linkid=2129500) ili [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).
1. [Povežite Windows računare sa uslugom Azure](https://go.microsoft.com/fwlink/?linkid=2129913). Nabavite ID radnog prostora i primarni ključ radnog prostora. Čarobnjaku za podešavanje potrebne su ove informacije da bi se propisno konfigurisao agent i da osigura komunikaciju sa Azure monitorom.
1. [Pritisnite podatke za dijagnostiku u radni prostor](https://go.microsoft.com/fwlink/?linkid=2128284). Možete da pritisnete podatke iz WVD stanara u analitiku evidencije za radni prostor.
1. [Identifikovanje i Dijagnostikovanje problema](https://go.microsoft.com/fwlink/?linkid=2128338) koji su unutrašnji ili spoljni u odnosu na wvd.

Da biste saznali više o konfigurisanju alatke za dijagnostiku usluge za WVD, pogledajte članak [Korišćenje analitike evidencije za funkciju dijagnostike](https://go.microsoft.com/fwlink/?linkid=2128084).
