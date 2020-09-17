---
title: Pitanja o korišćenju Office alatke za primenu (ODT)
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: e9f7581fd21cf5ca2d712038c4b73b67d08f3a76
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/15/2020
ms.locfileid: "47774905"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a>Pitanja o korišćenju Office alatke za primenu (ODT)

Preuzmite alatku za primenu sistema Office sa [lokacije Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).
  
Kada preuzmete datoteku, pokrećete datoteku samouvaštavanja koja sadrži alatku za Office primenu (setup.exe) i probnu datoteku konfiguracije (configuration.xml).
  
 **Da biste isključili ili uklonili Microsoft 365 aplikacije za Enterprise proizvode sa klijentskih računara:**
  
Kada instalirate Microsoft 365 aplikacije za Enterprise, možete da isključite specifične proizvode. Da biste to uradili, pratite korake za instaliranje sistema Office sa ODT, ali na datoteku konfiguracije dodajte ekskluzivni element. Na primer, ova Konfiguraciona datoteka instalira sve Microsoft 365 aplikacije za Enterprise proizvode osim izdavača:
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[Pregled alatke za primenu u sistemu Office](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)
  

