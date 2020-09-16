---
title: Kreiranje lokacije u usluzi SharePoint online
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 84f2b70e-2b23-4039-8305-85783798feed
ms.openlocfilehash: b554bfa4ccccbd68d0c3df27cf17397f860735c2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47732252"
---
# <a name="create-sharepoint-sites-using-templates"></a><span data-ttu-id="30c95-102">Kreiranje SharePoint lokacija pomoću predložaka</span><span class="sxs-lookup"><span data-stu-id="30c95-102">Create SharePoint sites using templates</span></span>

<span data-ttu-id="30c95-103">Mogućnost čuvanja lokacije kao predloška nije podržana uz modernu komunikaciju ili lokacije tima.</span><span class="sxs-lookup"><span data-stu-id="30c95-103">The ability to save a site as a template is not supported with modern Communication or Team Sites.</span></span> <span data-ttu-id="30c95-104">Više informacija o korišćenju predložaka potražite [u članku čuvanje i otpremanje SharePoint lokacije kao predloška](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template).</span><span class="sxs-lookup"><span data-stu-id="30c95-104">For more information about using templates see [Save, download and upload a SharePoint site as a template](https://docs.microsoft.com/sharepoint/dev/general-development/save-download-and-upload-a-sharepoint-site-as-a-template).</span></span>

<span data-ttu-id="30c95-105">Evo nekih uobičajenih problema/rešenja u vezi sa čuvanjem lokacije ili liste kao predloška u usluzi SharePoint online.</span><span class="sxs-lookup"><span data-stu-id="30c95-105">Here are some common issues/solutions regarding Saving a Site or List as a template in Sharepoint Online.</span></span> 

<span data-ttu-id="30c95-106">**Dugme "Sačuvaj predložak sajta/liste" nije dostupno ili nedostaje**</span><span class="sxs-lookup"><span data-stu-id="30c95-106">**Save site/list template button is not available or missing**</span></span>

<span data-ttu-id="30c95-107">Administratori će morati da dozvole prilagođenu skripcu za omogućavanje funkcija predloška.</span><span class="sxs-lookup"><span data-stu-id="30c95-107">Administrators will need to Allow Custom Script to enable the template features.</span></span> <span data-ttu-id="30c95-108">Detaljne korake, primeri i razmatranja</span><span class="sxs-lookup"><span data-stu-id="30c95-108">For detailed steps, examples and considerations see</span></span> 

- [<span data-ttu-id="30c95-109">Omogućavanje ili sprečavanje prilagođene skripte</span><span class="sxs-lookup"><span data-stu-id="30c95-109">Allow or prevent custom script</span></span>](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

- <span data-ttu-id="30c95-110">Komanda "Sačuvaj lokaciju kao predložak" nije podržana i može da izazove probleme na lokacijama koje koriste infrastrukturu za objavljivanje na SharePoint serveru.</span><span class="sxs-lookup"><span data-stu-id="30c95-110">The Save site as template command is not supported and can cause problems on sites that use the SharePoint Server Publishing Infrastructure.</span></span>

<span data-ttu-id="30c95-111">**Nije moguće kreirati predložak veb sajta ili ne funkcioniše ispravno**</span><span class="sxs-lookup"><span data-stu-id="30c95-111">**The site template cannot be created or does not work correctly**</span></span>

<span data-ttu-id="30c95-112">Predlošku možda nedostaje [funkcija](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) i neće se aktivirati.</span><span class="sxs-lookup"><span data-stu-id="30c95-112">The template may be missing a [feature](https://social.technet.microsoft.com/wiki/contents/articles/14423.sharepoint-2013-existing-features-guid.aspx) and won't activate.</span></span> <span data-ttu-id="30c95-113">Ako funkcija nije dostupna za aktiviranje trenutne kolekcije lokacija, ne možete da koristite predložak Veb lokacija da biste kreirali sajt.</span><span class="sxs-lookup"><span data-stu-id="30c95-113">If the feature is not available to activate in the current site collection, you cannot use the site template to create a site.</span></span>

- <span data-ttu-id="30c95-114">Potvrdite izbor u ovom polju za proveru da li bilo koje liste ili biblioteke premašuju [cenzus](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) od 5000 stavki pomoću kojih to može da blokira Kreiranje predloška sajta.</span><span class="sxs-lookup"><span data-stu-id="30c95-114">Check to see if any lists or libraries exceed the [List View Limit Threshold](https://support.office.com/article/Manage-large-lists-and-libraries-in-SharePoint-B8588DAE-9387-48C2-9248-C24122F07C59) of 5000 items as this can block creation of a site template.</span></span>

- <span data-ttu-id="30c95-115">Lokacija možda koristi previše resursa i samim tim, predložak sajta premašuje ograničenje od 50 MB.</span><span class="sxs-lookup"><span data-stu-id="30c95-115">The site may be using too many resources and therefore the site template exceeds the 50 MB limit.</span></span>


- <span data-ttu-id="30c95-116">Postoje problemi sa prikazivanjem podataka sa liste koja koristi kolonu za pronalaženje.</span><span class="sxs-lookup"><span data-stu-id="30c95-116">There are problems displaying data from a list that uses a lookup column.</span></span> <span data-ttu-id="30c95-117">Više informacija potražite u članku [lista sa obrascem koji je generisao ne pokazuje podatke sa odgovarajuće liste za pronalaženje u usluzi SharePoint online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span><span class="sxs-lookup"><span data-stu-id="30c95-117">For more information, see [Template-generated list doesn't display data from the correct lookup list in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/template-generated-list-incorrect-data).</span></span>

<span data-ttu-id="30c95-118">Detaljnije informacije o uobičajenim problemima i rešenjima potražite u okviru [Kreiranje i korišćenje predložaka lokacija](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span><span class="sxs-lookup"><span data-stu-id="30c95-118">For more detailed information on common problems and solutions, please check [Create and use site templates](https://support.office.com/article/Create-and-use-site-templates-60371B0F-00E0-4C49-A844-34759EBDD989).</span></span>



