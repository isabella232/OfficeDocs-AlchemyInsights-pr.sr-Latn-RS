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
ms.openlocfilehash: 9698aa12ad73a021a3cc12c8517c1712c48d8385
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/15/2020
ms.locfileid: "47794925"
---
# <a name="using-the-office-deployment-tool-odt"></a><span data-ttu-id="87aef-102">Korišćenje alatke za primenu u sistemu Office (ODT)</span><span class="sxs-lookup"><span data-stu-id="87aef-102">Using the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="87aef-103">Koristite Office alatku za primenu (ODT) da biste primenili Office 365 verzije sistema Office.</span><span class="sxs-lookup"><span data-stu-id="87aef-103">You use the Office Deployment Tool (ODT) to deploy Office 365 versions of Office.</span></span> <span data-ttu-id="87aef-104">Alatka "Office" za primenu (setup.exe) se pokreće sa komandne linije i koristi XML datoteku konfiguracije da bi odredila koje postavke treba da primenjuju prilikom primene sistema Office.</span><span class="sxs-lookup"><span data-stu-id="87aef-104">The Office Deployment Tool (setup.exe) is run from the command line and uses a configuration XML file to determine what settings to apply when deploying Office.</span></span>
  
1. <span data-ttu-id="87aef-105">Preuzmite najnoviju verziju alatke "Office" za primenu sa [lokacije Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="87aef-105">Download the latest version of the Office Deployment Tool from the [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>

2. <span data-ttu-id="87aef-106">Koristite [alatku za prilagođavanje sistema Office (OCT)](https://config.office.com) da biste izabrali željene postavke primene i kreirali XML datoteku konfiguracije.</span><span class="sxs-lookup"><span data-stu-id="87aef-106">Use the [Office Customization Tool (OCT)](https://config.office.com) to select your deployment preferences and create the configuration XML file.</span></span> <span data-ttu-id="87aef-107">Izvezite datoteku za konfiguraciju i stavite je lokalno u istu fasciklu u kojoj se nalazi setup.exe.</span><span class="sxs-lookup"><span data-stu-id="87aef-107">Export the configuration file and place it locally on the same folder where the setup.exe resides.</span></span>

    <span data-ttu-id="87aef-108">**Napomena:** Problemi sa instalacijom sistema Office obično se dešavaju zbog problema sa konfiguracionim datotekama za konfiguraciju.</span><span class="sxs-lookup"><span data-stu-id="87aef-108">**Note:** Office installation issues commonly occur due to misconfigured or malformatted configuration files.</span></span> <span data-ttu-id="87aef-109">Da biste izbegli takve probleme, preporučujemo da koristite alatku za prilagođavanje sistema Office da biste kreirali datoteku konfiguracije.</span><span class="sxs-lookup"><span data-stu-id="87aef-109">To avoid such issues, we recommend that you use the Office Customization Tool to create the configuration file.</span></span> <span data-ttu-id="87aef-110">Možete i da uvezete postojeće konfiguracione datoteke u alatku za prilagođavanje sistema Office.</span><span class="sxs-lookup"><span data-stu-id="87aef-110">You can also import existing configuration files into the Office Customization Tool.</span></span>

3. <span data-ttu-id="87aef-111">Sa otvorene komandne linije, prebacite se na lokaciju na kojoj setup.exe čuva i pokreće Office alatku za primenu u režimu preuzimanja i navedite datoteku za konfiguraciju koju ste upravo sačuvali.</span><span class="sxs-lookup"><span data-stu-id="87aef-111">From an elevated command prompt, switch to the location where setup.exe resides and run the Office Deployment Tool in download mode and specify the configuration file you just saved.</span></span> <span data-ttu-id="87aef-112">U ovom primeru, datoteka za konfiguraciju se zove Configuration.xml:</span><span class="sxs-lookup"><span data-stu-id="87aef-112">In this example, the configuration file is named Configuration.xml:</span></span>

```setup.exe /download Configuration.xml```

<span data-ttu-id="87aef-113">4. izvršite alatku za primenu sistema Office u režimu konfigurisanja i navedite datoteku za konfiguraciju.</span><span class="sxs-lookup"><span data-stu-id="87aef-113">4.Run the Office Deployment Tool in configure mode and specify the configuration file.</span></span>

```setup.exe /configure Configuration.xml```

<span data-ttu-id="87aef-114">**Napomena:** Morate da izvršite ovaj korake sa klijentskog računara na kojem želite da instalirate Office i morate da imate dozvole za lokalnu administratorsku dozvolu na tom računaru.</span><span class="sxs-lookup"><span data-stu-id="87aef-114">**Note:** You must run this step from the client computer on which you want to install Office and you must have local administrator permissions on that computer.</span></span>

<span data-ttu-id="87aef-115">Da biste saznali više o korišćenju Office alatke za primenu za Microsoft 365 aplikacije za scenarije primene preduzeća, pogledajte članak [pregled alatke za primenu sistema Office](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool).</span><span class="sxs-lookup"><span data-stu-id="87aef-115">To learn more about using Office Deployment Tool for your Microsoft 365 Apps for enterprise deployment scenarios, see [Overview of the Office Deployment Tool](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool).</span></span> <span data-ttu-id="87aef-116">Više detalja o tome kako da koristite alatku za prilagođavanje sistema Office potražite [u članku Pregled alatke za prilagođavanje sistema Office](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span><span class="sxs-lookup"><span data-stu-id="87aef-116">For more details on how to use the Office Customization Tool, see [Overview of the Office Customization Tool](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).</span></span>
