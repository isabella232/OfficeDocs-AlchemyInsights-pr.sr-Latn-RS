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
ms.openlocfilehash: c5b055989014b464d3136895702c8ea40e8eb701
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 11/17/2020
ms.locfileid: "49086170"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a><span data-ttu-id="9cffa-102">Pitanja o korišćenju Office alatke za primenu (ODT)</span><span class="sxs-lookup"><span data-stu-id="9cffa-102">Questions about how to use the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="9cffa-103">Preuzmite alatku za primenu sistema Office sa [lokacije Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="9cffa-103">Download the Office Deployment Tool from the [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>
  
<span data-ttu-id="9cffa-104">Kada preuzmete datoteku, pokrećete datoteku samouvaštavanja koja sadrži alatku za Office primenu (setupodt.exe) i probnu datoteku konfiguracije (configuration.xml).</span><span class="sxs-lookup"><span data-stu-id="9cffa-104">After downloading the file, run the self-extracting executable file, which contains the Office Deployment Tool executable (setupodt.exe) and a sample configuration file (configuration.xml).</span></span>
  
 <span data-ttu-id="9cffa-105">**Da biste isključili ili uklonili Microsoft 365 aplikacije za Enterprise proizvode sa klijentskih računara:**</span><span class="sxs-lookup"><span data-stu-id="9cffa-105">**To exclude or remove Microsoft 365 Apps for enterprise products from client computers:**</span></span>
  
<span data-ttu-id="9cffa-106">Kada instalirate Microsoft 365 aplikacije za Enterprise, možete da isključite specifične proizvode.</span><span class="sxs-lookup"><span data-stu-id="9cffa-106">When installing Microsoft 365 Apps for enterprise, you can exclude specific products.</span></span> <span data-ttu-id="9cffa-107">Da biste to uradili, pratite korake za instaliranje sistema Office sa ODT, ali na datoteku konfiguracije dodajte ekskluzivni element.</span><span class="sxs-lookup"><span data-stu-id="9cffa-107">To do so, follow the steps for installing Office with the ODT, but include the ExcludeApp element in your configuration file.</span></span> <span data-ttu-id="9cffa-108">Na primer, ova Konfiguraciona datoteka instalira sve Microsoft 365 aplikacije za Enterprise proizvode osim izdavača:</span><span class="sxs-lookup"><span data-stu-id="9cffa-108">For example, this configuration file installs all the Microsoft 365 Apps for enterprise products except Publisher:</span></span>
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[<span data-ttu-id="9cffa-109">Pregled alatke za primenu u sistemu Office</span><span class="sxs-lookup"><span data-stu-id="9cffa-109">Overview of the Office Deployment Tool</span></span>](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool)
  

