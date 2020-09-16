---
title: Upravljanje šemom pretrage u usluzi SharePoint online
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: f2d8d3e07fe32d21af484e4c59e0f5ac6fe8081c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/15/2020
ms.locfileid: "47770565"
---
# <a name="manage-search-schema-in-sharepoint-online"></a><span data-ttu-id="1c226-102">Upravljanje šemom pretrage u usluzi SharePoint online</span><span class="sxs-lookup"><span data-stu-id="1c226-102">Manage search schema in SharePoint Online</span></span>

<span data-ttu-id="1c226-103">Šema pretrage kontroliše šta korisnici mogu da traže, kako korisnici mogu da je pretražuju i kako da ih predstavite na Veb lokacijama za pretragu.</span><span class="sxs-lookup"><span data-stu-id="1c226-103">The search schema controls what users can search for, how users can search it, and how you can present the results on your search websites.</span></span> 

<span data-ttu-id="1c226-104">Pogledajte članak [Upravljanje šemom pretrage u usluzi SharePoint online](https://docs.microsoft.com/sharepoint/manage-search-schema) da biste saznali kako da:</span><span class="sxs-lookup"><span data-stu-id="1c226-104">See [Manage the Search Schema in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-search-schema) to learn how to:</span></span> 
- <span data-ttu-id="1c226-105">Promena šeme pretrage.</span><span class="sxs-lookup"><span data-stu-id="1c226-105">Change the search schema.</span></span>
- <span data-ttu-id="1c226-106">Kreirajte upravljana svojstva.</span><span class="sxs-lookup"><span data-stu-id="1c226-106">Create managed properties.</span></span>
- <span data-ttu-id="1c226-107">Mapiranje popisanih svojstava na popisanom svojstvima.</span><span class="sxs-lookup"><span data-stu-id="1c226-107">Map crawled map crawled properties to managed properties.</span></span>

<span data-ttu-id="1c226-108">Obratite pažnju na sledeće načine za upravljanje šemom pretrage:</span><span class="sxs-lookup"><span data-stu-id="1c226-108">Note the following in regards to managing your Search Schema:</span></span>

- <span data-ttu-id="1c226-109">Ako dobijete upozorenje koje navodi **da je aplikacija pauzirana** prilikom pravljenja promene šeme, to je privremeno samo ako se dešava održavanje usluge.</span><span class="sxs-lookup"><span data-stu-id="1c226-109">If you receive a warning stating **the application is paused** when making a schema change, this is only temporary as there is service maintenance occurring.</span></span> 

    <span data-ttu-id="1c226-110">Ako je prošlo više od 24 časa i još uvek doživite upozorenje, prijavite se u slučaju podrške.</span><span class="sxs-lookup"><span data-stu-id="1c226-110">If more than 24 hours have passed and you still experience the warning, please log a support case.</span></span>
- <span data-ttu-id="1c226-111">Kada promenite upravljana svojstva ili dodate nove, promene će stupiti na snagu tek kada se sadržaj ponovo satera.</span><span class="sxs-lookup"><span data-stu-id="1c226-111">When you change managed properties or add new ones, the changes take effect only after the content has been re-crawled.</span></span> <span data-ttu-id="1c226-112">U usluzi SharePoint online popisivanje se automatski odvija na osnovu definisanog rasporeda popisivanja.</span><span class="sxs-lookup"><span data-stu-id="1c226-112">In SharePoint Online, crawling happens automatically based on the defined crawl schedule.</span></span>
- <span data-ttu-id="1c226-113">Da biste se uverili da se promene popisuju, možete posebno da [zahtevate ponovno indeksiranje liste ili biblioteke](https://docs.microsoft.com/sharepoint/manage-search-schema#request-re-indexing-of-a-document-library-or-list)</span><span class="sxs-lookup"><span data-stu-id="1c226-113">To make sure that your changes are crawled, you can specifically [request a re-indexing of the list or library](https://docs.microsoft.com/sharepoint/manage-search-schema#request-re-indexing-of-a-document-library-or-list)</span></span> 

<span data-ttu-id="1c226-114">Potpun pregled šeme pretrage potražite u članku [upoznavanje šeme pretrage](https://blogs.technet.microsoft.com/tothesharepoint/2012/11/25/introducing-search-schema-for-sharepoint-2013/)</span><span class="sxs-lookup"><span data-stu-id="1c226-114">For a complete overview of the Search Schema, see [Introducing Search Schema](https://blogs.technet.microsoft.com/tothesharepoint/2012/11/25/introducing-search-schema-for-sharepoint-2013/)</span></span> 


