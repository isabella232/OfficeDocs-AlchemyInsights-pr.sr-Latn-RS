---
title: Korišćenje alatke Kancelarija za primenu
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
ms.openlocfilehash: 39a011d4b121492d222ff620e70d9860231b7bcfe0d7fd2ecfd93de1ef502f5f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "54083784"
---
# <a name="using-the-office-deployment-tool-odt"></a>Korišćenje alatke Kancelarija za primenu (ODT)

Alatku za Kancelarija primenu (ODT) koristite za Office 365 verzije sistema Kancelarija. Alatka Kancelarija za primenu (setup.exe) pokreće se sa komandne linije i koristi konfiguracionu XML datoteku da bi utvrdila koje postavke treba primeniti prilikom primene programa Kancelarija.
  
1. Preuzmite najnoviju verziju alatke Kancelarija za primenu sa [lokacije Microsoft Download Center.](https://go.microsoft.com/fwlink/p/?LinkID=626065)

2. Koristite [alatku Kancelarija za prilagođavanje (OCT)](https://config.office.com) da biste izabrali željene postavke primene i napravili XML datoteku konfiguracije. Izvezite konfiguracionu datoteku i stavite je lokalno u istu fasciklu u kojoj se setup.exe nalazi.

    **Napokon:** Kancelarija problema sa instalacijom obično dolazi zbog neiskonfigurisanih ili neoblikiranih datoteka konfiguracije. Da biste izbegli takve probleme, preporučujemo da koristite alatku Kancelarija za prilagođavanje da biste napravili konfiguracionu datoteku. U alatku za prilagođavanje možete da uvezete i postojeće konfiguracione datoteke Kancelarija alatki za prilagođavanje.

3. Sa komandne linije sa punim veličinama prebacite se na lokaciju na kojoj setup.exe nalazite i pokrenite alatku za Kancelarija za primenu u režimu preuzimanja i navedite konfiguracionu datoteku koju ste upravo sačuvali. U ovom primeru, konfiguraciona datoteka se zove Configuration.xml:

```setup.exe /download Configuration.xml```

4.Pokrenite alatku Kancelarija za primenu u režimu konfigurisanja i navedite datoteku konfiguracije.

```setup.exe /configure Configuration.xml```

**Napomogućeno:** Ovaj korak morate da pokrenete sa klijentskog računara na kojem želite da instalirate Kancelarija i morate da imate lokalne administratorske dozvole na tom računaru.

Da biste saznali više o korišćenju Kancelarija alatke za primenu za scenarije Microsoft 365 Apps za preduzeće primene, pogledajte pregled alatke [za Kancelarija primenu.](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool) Za više detalja o tome kako da koristite alatku Kancelarija za prilagođavanje pogledajte pregled [alatke Kancelarija za prilagođavanje.](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run)
