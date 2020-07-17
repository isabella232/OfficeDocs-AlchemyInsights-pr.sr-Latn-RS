---
title: isto kao i ime datoteke je najbolje
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: bd2901580acdb1dc17f3e14a7a9356b07e70f910
ms.sourcegitcommit: bf6a0e80d09aebae19b9e993c2552b88e49177c9
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 06/16/2020
ms.locfileid: "44750984"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="6ea1e-102">"Zahtevano Alhemy zaglavlje H1, H2's ne funkcionišu."</span><span class="sxs-lookup"><span data-stu-id="6ea1e-102">"Required Alchemy Header H1, H2's dont work."</span></span>
<span data-ttu-id="6ea1e-103">Najbolja praksa i uputstava za Alhemy kreiranje:</span><span class="sxs-lookup"><span data-stu-id="6ea1e-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="6ea1e-104">**Ne ugnezdite Alhemy opažanja u fasciklama**-ovo će prekinuti strukturu URL adrese.</span><span class="sxs-lookup"><span data-stu-id="6ea1e-104">**Do not nest Alchemy Insights in folders**- this will break the url structure.</span></span> <span data-ttu-id="6ea1e-105">Očekujemo da to ispravimo.</span><span class="sxs-lookup"><span data-stu-id="6ea1e-105">We're looking into fixing this.</span></span>
1. <span data-ttu-id="6ea1e-106">Datoteke u fascikli **Alhemyopažanja** bi trebalo da imaju mala slova sa crtica za razmake.</span><span class="sxs-lookup"><span data-stu-id="6ea1e-106">Files in the **AlchemyInsights** folder should have lowercase filenames with hyphens for spaces ex.</span></span> <span data-ttu-id="6ea1e-107">***Kako-to-Omogućivanje-održavanje***.</span><span class="sxs-lookup"><span data-stu-id="6ea1e-107">***how-to-enable-litigation-hold***.</span></span>
    1. <span data-ttu-id="6ea1e-108">Uključivanje ID-a ili ID-a u kantu sa [Alhemy partnerski portala](https://alchemyportal.azurewebsites.net) u polje "MS. Prilagođeno".</span><span class="sxs-lookup"><span data-stu-id="6ea1e-108">Include the Rule ID or bucket ID from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the ms.custom field.</span></span> <span data-ttu-id="6ea1e-109">Bivљi.</span><span class="sxs-lookup"><span data-stu-id="6ea1e-109">ex.</span></span> <span data-ttu-id="6ea1e-110">***Ms. prilagođen: 100021***</span><span class="sxs-lookup"><span data-stu-id="6ea1e-110">***ms.custom: 100021***</span></span>
1. <span data-ttu-id="6ea1e-111">Koristite ostale metapodatke na vrhu ove datoteke kao predložak.</span><span class="sxs-lookup"><span data-stu-id="6ea1e-111">Use the rest of the metadata at the top of this file as your template.</span></span>
1. <span data-ttu-id="6ea1e-112">U okviru [Alhemy partnera portala](https://alchemyportal.azurewebsites.net), krećite se do sekcije " **korisnički naslov uvida":** i koristite to kao polaznu tačku za vaš H1 naslov za uvid.</span><span class="sxs-lookup"><span data-stu-id="6ea1e-112">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="6ea1e-113">Alhemy opažanja mora imati samo jedan H1 na vrhu ili će se slomiti u proizvodnji.</span><span class="sxs-lookup"><span data-stu-id="6ea1e-113">Alchemy Insights MUST have only a single H1 at the top or they will break in production.</span></span> <span data-ttu-id="6ea1e-114">H2s nemojte da koristite **podebljane** ili druge konvencije da biste označili odvojene sekcije.</span><span class="sxs-lookup"><span data-stu-id="6ea1e-114">H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="6ea1e-115">Zatim, popunite telo teksta pomoću nacrta materijala u odeljku "pravilo o korisniku Alhemy"</span><span class="sxs-lookup"><span data-stu-id="6ea1e-115">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="6ea1e-116">Liste sa znakovima za nabrajanje su u redu</span><span class="sxs-lookup"><span data-stu-id="6ea1e-116">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="6ea1e-117">Numerisane liste takođe</span><span class="sxs-lookup"><span data-stu-id="6ea1e-117">Numbered lists too</span></span>
    1. <span data-ttu-id="6ea1e-118">**Podebljano** i *kurziv* su u redu</span><span class="sxs-lookup"><span data-stu-id="6ea1e-118">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="6ea1e-119">Veze uvek treba da budu **"veze ka Web"/eksternim** ili **dubokim vezama sa elementima korisničkog interfejsa**, a ne sa unutrašnjim vezama.</span><span class="sxs-lookup"><span data-stu-id="6ea1e-119">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>
    1. <span data-ttu-id="6ea1e-120">Slike trenutno nisu zvanično podržane, ali je na mapi.</span><span class="sxs-lookup"><span data-stu-id="6ea1e-120">Pictures are not officially supported at this time, but it's on the roadmap.</span></span>

<span data-ttu-id="6ea1e-121">A ovo je već malo predugo.</span><span class="sxs-lookup"><span data-stu-id="6ea1e-121">And this is really already a bit too long.</span></span> <span data-ttu-id="6ea1e-122">Najbolja praksa je oko 400 karaktera---------------------------------</span><span class="sxs-lookup"><span data-stu-id="6ea1e-122">Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="6ea1e-123">Kada je sadržaj spreman, povucite ga u Live granu.</span><span class="sxs-lookup"><span data-stu-id="6ea1e-123">Once your content is ready, pull it to the live branch.</span></span> <span data-ttu-id="6ea1e-124">Zatim idite na portal " [Alhemy partner](https://alchemyportal.azurewebsites.net) " i unesite ime u polje URL adrese.</span><span class="sxs-lookup"><span data-stu-id="6ea1e-124">Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field.</span></span> 