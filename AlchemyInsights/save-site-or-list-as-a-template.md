---
title: Čuvanje stranice ili liste kao predloška
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 368ff1fa-82cf-4a07-986e-140b212ffc5c
ms.openlocfilehash: 37ae727aa6dd6af94d0d833ce972aec413d90194
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727545"
---
# <a name="save-site-or-list-as-a-template"></a><span data-ttu-id="78b7c-102">Čuvanje stranice ili liste kao predloška</span><span class="sxs-lookup"><span data-stu-id="78b7c-102">Save site or list as a template</span></span>

<span data-ttu-id="78b7c-103">Predlošci SharePoint lokacije su unapred izgrađeni definicijedizajnirani oko određenih poslovnih potreba.</span><span class="sxs-lookup"><span data-stu-id="78b7c-103">SharePoint site templates are prebuilt definitions designed around a particular business need.</span></span> <span data-ttu-id="78b7c-104">Više informacija potražite u članku [Korišćenje predložaka za kreiranje raznih vrsta SharePoint lokacija](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span><span class="sxs-lookup"><span data-stu-id="78b7c-104">For more information, see [Using templates to create different kinds of SharePoint sites](https://support.office.com/article/using-templates-to-create-different-kinds-of-sharepoint-sites-449eccec-ff99-4cf3-b62e-dcfee37e8da4).</span></span>

<span data-ttu-id="78b7c-105">Evo nekih uobičajenih problema/rešenja u vezi sa čuvanjem lokacije ili liste kao predloška u usluzi SharePoint online.</span><span class="sxs-lookup"><span data-stu-id="78b7c-105">Here are some common issues/solutions regarding Saving a Site or List as a template in SharePoint Online.</span></span>

<span data-ttu-id="78b7c-106">**Dugme "Sačuvaj predložak sajta/liste" nije dostupno ili nedostaje**.</span><span class="sxs-lookup"><span data-stu-id="78b7c-106">**Save site/list template button is not available or missing**.</span></span> 

- <span data-ttu-id="78b7c-107">Administratori će morati da dozvole prilagođenu skripcu za omogućavanje funkcija predloška.</span><span class="sxs-lookup"><span data-stu-id="78b7c-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="78b7c-108">Detaljniji koraci, primeri i problemi vide [Omogućavanje ili sprečavanje prilagođenog skriptova](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span><span class="sxs-lookup"><span data-stu-id="78b7c-108">For detailed steps, examples and considerations see [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>


- <span data-ttu-id="78b7c-109">Komanda "Sačuvaj lokaciju kao predložak" nije podržana i može da izazove probleme na lokacijama koje koriste infrastrukturu za objavljivanje na SharePoint serveru.</span><span class="sxs-lookup"><span data-stu-id="78b7c-109">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>


<span data-ttu-id="78b7c-110">**Nije moguće kreirati predložak veb sajta ili ne funkcioniše ispravno**</span><span class="sxs-lookup"><span data-stu-id="78b7c-110">**The site template cannot be created or does not work correctly**</span></span>

- <span data-ttu-id="78b7c-111">Predlošku možda nedostaje [funkcija](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) i neće se aktivirati.</span><span class="sxs-lookup"><span data-stu-id="78b7c-111">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won’t activate.</span></span> <span data-ttu-id="78b7c-112">Ako funkcija nije dostupna za aktiviranje trenutne kolekcije lokacija, ne možete da koristite predložak Veb lokacija da biste kreirali sajt.</span><span class="sxs-lookup"><span data-stu-id="78b7c-112">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>


- <span data-ttu-id="78b7c-113">Potvrdite izbor u ovom polju za proveru da li bilo koje liste ili biblioteke premašuju [cenzus](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) od 5000 stavki pomoću kojih to može da blokira Kreiranje predloška sajta.</span><span class="sxs-lookup"><span data-stu-id="78b7c-113">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>


- <span data-ttu-id="78b7c-114">Lokacija možda koristi previše resursa i samim tim, predložak sajta premašuje ograničenje od 50 megabajta (MB).</span><span class="sxs-lookup"><span data-stu-id="78b7c-114">The site may be using too many resources and therefore the site template exceeds the 50 megabyte (MB) limit.</span></span>


- <span data-ttu-id="78b7c-115">Postoje problemi sa prikazivanjem podataka sa liste koja koristi kolonu za pronalaženje.</span><span class="sxs-lookup"><span data-stu-id="78b7c-115">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="78b7c-116">Više informacija potražite u članku [lista sa obrascem koji je generisao ne pokazuje podatke sa odgovarajuće liste za pronalaženje u usluzi SharePoint online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span><span class="sxs-lookup"><span data-stu-id="78b7c-116">For more information, see [Template-generated list doesn’t display data from the correct lookup list in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span></span>


<span data-ttu-id="78b7c-117">Detaljnije informacije o uobičajenim problemima i rešenjima navedite, [Kreirajte i koristite predloške lokacija](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span><span class="sxs-lookup"><span data-stu-id="78b7c-117">For more detailed information on common problems and solutions please reference, [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>

