---
title: Moderna lokacija kao osnovna lokacija
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ms.date: 04/21/2020
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: 86ff5f7fbaed62de9047006bf4ba4d2db2be3def
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47666884"
---
# <a name="modern-site-as-root-site"></a><span data-ttu-id="f2acb-102">Savremena lokacija kao osnovna lokacija</span><span class="sxs-lookup"><span data-stu-id="f2acb-102">Modern site as root site</span></span>

<span data-ttu-id="f2acb-103">Počeli smo da ovodimo novu funkciju koja će vam omogućiti da [zamenite klasičnu osnovnu veb sajt sajta modernom lokacijom](https://docs.microsoft.com/sharepoint/modern-root-site).</span><span class="sxs-lookup"><span data-stu-id="f2acb-103">We have begun to rollout a new feature that will allow you to [swap your classic site root site with a modern site](https://docs.microsoft.com/sharepoint/modern-root-site).</span></span> <span data-ttu-id="f2acb-104">Korišćenje poziva [-Spositesvp](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) za razmenu lokacije sa drugom lokacijom dok arhivirate originalnu lokaciju.</span><span class="sxs-lookup"><span data-stu-id="f2acb-104">Use [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) to swap the location of a site with another site while archiving the original site.</span></span> <span data-ttu-id="f2acb-105">Dostupno za oba sajta tima (nije povezano sa grupom) i sajt za komunikaciju.</span><span class="sxs-lookup"><span data-stu-id="f2acb-105">Available for both Team Site (not connected to a group) and Communication Site.</span></span>

>[!Important]
> <span data-ttu-id="f2acb-106">Nemojte da izbrišete klasičnu osnovnu sajt da biste kreirali modernu sajt za komunikaciju.</span><span class="sxs-lookup"><span data-stu-id="f2acb-106">Do not delete your classic root site to create a modern Communication Site.</span></span> <span data-ttu-id="f2acb-107">Microsoft ne podržava ovo.</span><span class="sxs-lookup"><span data-stu-id="f2acb-107">This is not supported by Microsoft.</span></span> <span data-ttu-id="f2acb-108">Brisanje osnovne lokacije će učiniti da sve SharePoint lokacije u vašoj organizaciji budu nedostupne svim korisnicima dok ne vratite lokaciju ili kreirate novu lokaciju na istoj URL adresi.</span><span class="sxs-lookup"><span data-stu-id="f2acb-108">Deleting the root site will make all SharePoint sites in your organization inaccessible to all users, until you restore the site or create a new site at the same URL.</span></span> <span data-ttu-id="f2acb-109">Ovu funkciju ćemo komunicirati putem centra za poruke.</span><span class="sxs-lookup"><span data-stu-id="f2acb-109">We’ll be communicating this feature via the message center.</span></span> <span data-ttu-id="f2acb-110">Trebalo bi da očekujete da će funkcija uskoro biti uključena u zakupca.</span><span class="sxs-lookup"><span data-stu-id="f2acb-110">You should expect the feature to be turned on in your tenant shortly.</span></span>

## <a name="known-issues-with-swapping-sites"></a><span data-ttu-id="f2acb-111">Poznati problemi sa Veb lokacijama</span><span class="sxs-lookup"><span data-stu-id="f2acb-111">Known issues with swapping sites</span></span>
- <span data-ttu-id="f2acb-112">Ciljna lokacija može da vrati grešku "nije pronađena" (HTTP 404) na kratko vreme.</span><span class="sxs-lookup"><span data-stu-id="f2acb-112">The target site may return a "not found" (HTTP 404) error for a short period of time.</span></span>
- <span data-ttu-id="f2acb-113">Potrebno je ponovo popisivati sadržaj da biste ažurirali indeks pretrage.</span><span class="sxs-lookup"><span data-stu-id="f2acb-113">Content will need to be recrawled to update the search index.</span></span> <span data-ttu-id="f2acb-114">Ovde ne postoji potreban ručni korake, ovo će biti gotovo automatski.</span><span class="sxs-lookup"><span data-stu-id="f2acb-114">There is no manual step required here, this will be done automatically.</span></span>
- <span data-ttu-id="f2acb-115">Sve što zavisi od veza "statične" (kao što su sinhronizacija datoteka i OneNote datoteke) mora se ručno ispraviti.</span><span class="sxs-lookup"><span data-stu-id="f2acb-115">Anything dependent on "static" links (such as File Sync and OneNote files) will need to be manually corrected.</span></span>
- <span data-ttu-id="f2acb-116">Za lokacije servera projekta možda će biti potrebno da se verifikujete da biste se uverili da su i dalje ispravno povezane.</span><span class="sxs-lookup"><span data-stu-id="f2acb-116">Project Server sites may need to be validated to ensure that they are still associated correctly.</span></span> 
