---
title: Razmena klasične osnovne sajta uz modernu sajt
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: 10e8e4bf5e0def9a8256066e1a3c39b9923d31b0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47691193"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a><span data-ttu-id="d2b76-102">Razmena klasične osnovne sajta uz modernu sajt</span><span class="sxs-lookup"><span data-stu-id="d2b76-102">Swap your Classic root site with a Modern site</span></span>

<span data-ttu-id="d2b76-103">Ako je okruženje podešeno pre 2019 aprila, možete da promenite osnovnu lokaciju na modernu lokaciju pomoću programa Microsoft PowerShell:</span><span class="sxs-lookup"><span data-stu-id="d2b76-103">If your environment was set up before April 2019, you can change your root site to a modern site by using Microsoft PowerShell:</span></span>

- <span data-ttu-id="d2b76-104">Ako imate različitu stranicu koju želite da koristite kao osnovnu sajt, možete da je zamenite [(zamijenite) osnovnu sajt](https://docs.microsoft.com/sharepoint/modern-root-site) sa njom.</span><span class="sxs-lookup"><span data-stu-id="d2b76-104">If you have a different site that you want to use as your root site, you can replace [(swap) the root site](https://docs.microsoft.com/sharepoint/modern-root-site) with it.</span></span> 
    - <span data-ttu-id="d2b76-105">Korišćenje poziva [-Spositesvp](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) za razmenu lokacije sa drugom lokacijom dok arhivirate originalnu lokaciju.</span><span class="sxs-lookup"><span data-stu-id="d2b76-105">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="d2b76-106">Dostupno za oba sajta tima (nije povezano sa grupom) i sajt za komunikaciju.</span><span class="sxs-lookup"><span data-stu-id="d2b76-106">Available for both Team Site (not connected to a group) and Communication Site.</span></span> 

- <span data-ttu-id="d2b76-107">Uskoro će biti predstavljene dodatne mogućnosti koje će vam omogućiti da nastavite da koristite sadržaj na sajtu, ali da konvertujete postojeću Veb na sajt za komunikaciju.</span><span class="sxs-lookup"><span data-stu-id="d2b76-107">Additional capabilities will be introduced soon that will allow you to keep using the content on the site, but convert the existing site to a communication site.</span></span> 
>[!Important]
><span data-ttu-id="d2b76-108">Ove mogućnosti će se postepeno razraditi.</span><span class="sxs-lookup"><span data-stu-id="d2b76-108">These capabilities will be rolled out gradually.</span></span> <span data-ttu-id="d2b76-109">Nastavite da proveravate centar za poruke za ispravke.</span><span class="sxs-lookup"><span data-stu-id="d2b76-109">Continue to check the Message Center for updates.</span></span> 

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="d2b76-110">Poznati problemi sa Veb lokacijama</span><span class="sxs-lookup"><span data-stu-id="d2b76-110">Known issues with swapping sites</span></span>

- <span data-ttu-id="d2b76-111">Ciljna lokacija može da vrati grešku "nije pronađena" (HTTP 404) na kratko vreme.</span><span class="sxs-lookup"><span data-stu-id="d2b76-111">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="d2b76-112">Potrebno je ponovo popisivati sadržaj da biste ažurirali indeks pretrage.</span><span class="sxs-lookup"><span data-stu-id="d2b76-112">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="d2b76-113">Ne postoji potreban ručni korake – ovo će biti gotovo automatski.</span><span class="sxs-lookup"><span data-stu-id="d2b76-113">There is no manual step required - this will be done automatically.</span></span>
- <span data-ttu-id="d2b76-114">Sve što zavisi od veza "statične" (kao što su sinhronizacija datoteka i OneNote datoteke) mora se ručno ispraviti.</span><span class="sxs-lookup"><span data-stu-id="d2b76-114">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="d2b76-115">Ako je izvorna lokacija bila organizaciona lokacija, ažurirajte URL.</span><span class="sxs-lookup"><span data-stu-id="d2b76-115">If the source site was an organizational news site, update the URL.</span></span><span data-ttu-id="d2b76-116">Nabavite listu svih sajtova za organizacije.</span><span class="sxs-lookup"><span data-stu-id="d2b76-116"> Get a list of all organizational news sites.</span></span>
- <span data-ttu-id="d2b76-117">Za lokacije servera projekta možda će biti potrebno da se verifikujete da biste se uverili da su i dalje ispravno povezane.</span><span class="sxs-lookup"><span data-stu-id="d2b76-117">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span>
