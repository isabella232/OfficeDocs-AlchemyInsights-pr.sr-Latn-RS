---
title: Pitanja o tome kako se koristi alatka Kancelarija za primenu (ODT)
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
ms.openlocfilehash: d38866647c7bf286b5b5b21e7fdcc94af72ea1850bc40391af077aa230b8b4fd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "53959697"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>Pitanja o tome kako se koristi alatka Kancelarija za primenu (ODT)

Preuzmite alatku Kancelarija za primenu sa [lokacije Microsoft Download Center.](https://go.microsoft.com/fwlink/p/?LinkID=626065)
  
Kada preuzmete datoteku, pokrenite samu izdvajanju izvršnu datoteku koja sadrži izvršnu datoteku Kancelarija Alatke za primenu (setup.exe) i uzorak datoteke konfiguracije (configuration.xml).
  
 **Da biste izuzeli ili Microsoft 365 Apps za preduzeće iz klijentskih računara:**
  
Prilikom instalacije Microsoft 365 Apps za preduzeće možete da isključite određene proizvode. Da biste to uradio, pratite korake za instaliranje datoteke Kancelarija ODT, ali uključite element ExcludeApp u konfiguracionu datoteku. Na primer, ova konfiguraciona datoteka instalira sve Microsoft 365 Apps za preduzeće osim Publisher:
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[Pregled alatke za Kancelarija primenu](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)
  

