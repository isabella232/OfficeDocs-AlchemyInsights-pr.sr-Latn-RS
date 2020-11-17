---
title: Korišćenje alatke za primenu sistema Office
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "918"
- "2000022"
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: f3a5dbfc6b64ccd4f0b19a5f86236336e78838d4
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 11/17/2020
ms.locfileid: "49085846"
---
# <a name="using-the-office-deployment-tool-odt"></a>Korišćenje alatke za primenu u sistemu Office (ODT)

Koristite Office alatku za primenu (ODT) da biste primenili Office 365 verzije sistema Office. Alatka "Office" za primenu (setupodt.exe) se pokreće sa komandne linije i koristi XML datoteku konfiguracije da bi odredila koje postavke treba da primenjuju prilikom primene sistema Office.
  
1. Preuzmite najnoviju verziju alatke "Office" za primenu sa [lokacije Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).

2. Koristite [alatku za prilagođavanje sistema Office (OCT)](https://config.office.com) da biste izabrali željene postavke primene i kreirali XML datoteku konfiguracije. Izvezite datoteku za konfiguraciju i stavite je lokalno u istu fasciklu u kojoj se nalazi setupodt.exe.

    **Napomena:** Problemi sa instalacijom sistema Office obično se dešavaju zbog problema sa konfiguracionim datotekama za konfiguraciju. Da biste izbegli takve probleme, preporučujemo da koristite alatku za prilagođavanje sistema Office da biste kreirali datoteku konfiguracije. Možete i da uvezete postojeće konfiguracione datoteke u alatku za prilagođavanje sistema Office.

3. Sa otvorene komandne linije, prebacite se na lokaciju na kojoj setupodt.exe čuva i pokreće Office alatku za primenu u režimu preuzimanja i navedite datoteku za konfiguraciju koju ste upravo sačuvali. U ovom primeru, datoteka za konfiguraciju se zove Configuration.xml:

```setupodt.exe /download Configuration.xml```

4. izvršite alatku za primenu sistema Office u režimu konfigurisanja i navedite datoteku za konfiguraciju.

```setupodt.exe /configure Configuration.xml```

**Napomena:** Morate da izvršite ovaj korake sa klijentskog računara na kojem želite da instalirate Office i morate da imate dozvole za lokalnu administratorsku dozvolu na tom računaru.

Da biste saznali više o korišćenju Office alatke za primenu za Microsoft 365 aplikacije za scenarije primene preduzeća, pogledajte članak [pregled alatke za primenu sistema Office](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool). Više detalja o tome kako da koristite alatku za prilagođavanje sistema Office potražite [u članku Pregled alatke za prilagođavanje sistema Office](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).
