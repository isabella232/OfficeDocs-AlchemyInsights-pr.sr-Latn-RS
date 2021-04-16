---
title: Pitanja o tome kako se koristi alatka za primenu programnog sistema Office (ODT)
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: 20e0b6aa3c298ee0a4291c3da6ae46978177e81f
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/15/2021
ms.locfileid: "51790346"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>Pitanja o tome kako se koristi alatka za primenu programnog sistema Office (ODT)

Preuzmite alatku za primenu programskog paketa Office sa [lokacije Microsoft Download Center.](https://go.microsoft.com/fwlink/p/?LinkID=626065)
  
Kada preuzmete datoteku, pokrenite samu izdvajanju izvršnu datoteku koja sadrži izvršnu datoteku alatke za primenu programnog sistema Office (setup.exe) i uzorak konfiguracione datoteke (configuration.xml).
  
 **Da biste izuzeli ili uklonili Microsoft 365 aplikacije za poslovne proizvode sa klijentskih računara:**
  
Prilikom instaliranja Microsoft 365 aplikacija za preduzeća, možete da isključite određene proizvode. Da biste to uradio, pratite korake za instaliranje sistema Office sa ODT datotekom, ali uključite element ExcludeApp u konfiguracionu datoteku. Na primer, ova konfiguraciona datoteka instalira sve Microsoft 365 aplikacije za poslovne proizvode osim programa Publisher:
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[Pregled alatke za primenu programnog sistema Office](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)
  

