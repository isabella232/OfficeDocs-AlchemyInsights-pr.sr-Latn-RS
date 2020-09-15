---
title: isto kao što je ime datoteke najbolje
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: 113d01e0fc92cc9845e585919ab05f386d6892bb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664148"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="16ecc-102">"Obavezno Alhemimy zaglavlje H1, H2's ne funkcioniše".</span><span class="sxs-lookup"><span data-stu-id="16ecc-102">"Required Alchemy Header H1, H2's dont work."</span></span>
<span data-ttu-id="16ecc-103">Najbolje prakse i uputstva za kreiranje alhemije:</span><span class="sxs-lookup"><span data-stu-id="16ecc-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="16ecc-104">**Ne gnezdite se po alhemiji u fasciklama**– ovo će prekinuti strukturu URL adrese.</span><span class="sxs-lookup"><span data-stu-id="16ecc-104">**Do not nest Alchemy Insights in folders**- this will break the url structure.</span></span> <span data-ttu-id="16ecc-105">Traћimo da ovo popravimo.</span><span class="sxs-lookup"><span data-stu-id="16ecc-105">We're looking into fixing this.</span></span>
1. <span data-ttu-id="16ecc-106">Datoteke u fascikli " **Alhemimiinsajd** " trebalo bi da imaju mala polja sa crtima za razmake za razmak.</span><span class="sxs-lookup"><span data-stu-id="16ecc-106">Files in the **AlchemyInsights** folder should have lowercase filenames with hyphens for spaces ex.</span></span> <span data-ttu-id="16ecc-107">***Kako-to-omogućiti-čekanje***.</span><span class="sxs-lookup"><span data-stu-id="16ecc-107">***how-to-enable-litigation-hold***.</span></span>
    1. <span data-ttu-id="16ecc-108">Uključujete ID pravila ili ID za kantu sa [portala Alhemimy partner](https://alchemyportal.azurewebsites.net) u polju MS. prilagođeno.</span><span class="sxs-lookup"><span data-stu-id="16ecc-108">Include the Rule ID or bucket ID from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the ms.custom field.</span></span> <span data-ttu-id="16ecc-109">odgovora.</span><span class="sxs-lookup"><span data-stu-id="16ecc-109">ex.</span></span> <span data-ttu-id="16ecc-110">***Ms. Custom: 100021***</span><span class="sxs-lookup"><span data-stu-id="16ecc-110">***ms.custom: 100021***</span></span>
1. <span data-ttu-id="16ecc-111">Koristite ostatak metapodataka na vrhu datoteke kao predložak.</span><span class="sxs-lookup"><span data-stu-id="16ecc-111">Use the rest of the metadata at the top of this file as your template.</span></span>
1. <span data-ttu-id="16ecc-112">Na [portalu Alhemijmy za partnere](https://alchemyportal.azurewebsites.net)se pomerite do naslova odeljka " **Inrubrika klijenta":** i koristite ga kao početnu vrednost za H1 naslov za uvid.</span><span class="sxs-lookup"><span data-stu-id="16ecc-112">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="16ecc-113">Pronicljivost alhemije mora da ima samo jedan H1 na vrhu ili će se probiti u proizvodnji.</span><span class="sxs-lookup"><span data-stu-id="16ecc-113">Alchemy Insights MUST have only a single H1 at the top or they will break in production.</span></span> <span data-ttu-id="16ecc-114">H2s ne daje tako da koristi **podebljano** ili druge konvencije za označavanje odvojenih odeljaka.</span><span class="sxs-lookup"><span data-stu-id="16ecc-114">H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="16ecc-115">Pored toga, unesite tekst u telo koristeći materijal za radnu verziju u odeljku "uvid u klijenta" na stranici "Alhemimy pravilo"</span><span class="sxs-lookup"><span data-stu-id="16ecc-115">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="16ecc-116">Liste sa znakovima za nabrajanje su dobre</span><span class="sxs-lookup"><span data-stu-id="16ecc-116">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="16ecc-117">Takođe i numerisane liste</span><span class="sxs-lookup"><span data-stu-id="16ecc-117">Numbered lists too</span></span>
    1. <span data-ttu-id="16ecc-118">**Podebljano** i *kurziv* su u redu</span><span class="sxs-lookup"><span data-stu-id="16ecc-118">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="16ecc-119">Veze bi uvek trebalo da budu **"veze ka vebu"/spoljnje** ili **duboke veze sa elementima korisničkog interfejsa**, a ne sa unutrašnjim vezama.</span><span class="sxs-lookup"><span data-stu-id="16ecc-119">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>
    1. <span data-ttu-id="16ecc-120">Slike trenutno nisu podržane, ali je na mapi.</span><span class="sxs-lookup"><span data-stu-id="16ecc-120">Pictures are not officially supported at this time, but it's on the roadmap.</span></span>

<span data-ttu-id="16ecc-121">Ovo je već malo predugačko.</span><span class="sxs-lookup"><span data-stu-id="16ecc-121">And this is really already a bit too long.</span></span> <span data-ttu-id="16ecc-122">Najbolja praksa je oko 400 znakova---------------------------------</span><span class="sxs-lookup"><span data-stu-id="16ecc-122">Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="16ecc-123">Kada se sadržaj pripremi, povucite ga na granu uživo.</span><span class="sxs-lookup"><span data-stu-id="16ecc-123">Once your content is ready, pull it to the live branch.</span></span> <span data-ttu-id="16ecc-124">Zatim idite na portal sa [Alhemimemojim partnerom](https://alchemyportal.azurewebsites.net) i unesite ime u polje URL adresa.</span><span class="sxs-lookup"><span data-stu-id="16ecc-124">Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field.</span></span> 