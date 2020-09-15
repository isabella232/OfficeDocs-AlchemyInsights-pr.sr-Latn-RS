---
title: Dynamics 365-pogrešan instrument Kontrolna tabla u programu Dynamics 365 objedinjeno interfejs
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1484"
- "6200024"
ms.openlocfilehash: 02e33c7dbdfe9b7d2ad7a04f154cf067fba0aab2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47711289"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a><span data-ttu-id="8e8c2-102">Pogrešna Kontrolna tabla prikazuje u dinamici Dynamics 365</span><span class="sxs-lookup"><span data-stu-id="8e8c2-102">Wrong dashboard shows in Dynamics 365 unified interface</span></span>

<span data-ttu-id="8e8c2-103">Postoji nekoliko razloga zbog kojih možete da vidite drugu kontrolnu tablu od one koju očekujete:</span><span class="sxs-lookup"><span data-stu-id="8e8c2-103">There are several reasons why you may see a different dashboard than the one you expect:</span></span>

## <a name="the-user-has-set-a-user-default-dashboard"></a><span data-ttu-id="8e8c2-104">Korisnik je podesio podrazumevani instrument-tablu</span><span class="sxs-lookup"><span data-stu-id="8e8c2-104">The user has set a user default dashboard</span></span> 

<span data-ttu-id="8e8c2-105">Najčešće možete identifikovati korisničku početnu kontrolnu tablu ako se dugme **Postavi kao podrazumevano** ne prikaže na komandnoj traci kontrolne table.</span><span class="sxs-lookup"><span data-stu-id="8e8c2-105">Typically you can identify a user default dashboard is set if the **Set As Default** button does not show in the dashboard command bar.</span></span> <span data-ttu-id="8e8c2-106">Kontrolna tabla korisnika će zameniti sve druge podrazumevane kontrolne table, čak i ako podrazumevana Kontrolna tabla korisnika nije u trenutnoj aplikaciji.</span><span class="sxs-lookup"><span data-stu-id="8e8c2-106">The user default dashboard will override all other default dashboards, even if the user's default dashboard is not in the current app.</span></span>

<span data-ttu-id="8e8c2-107">Koristite sledeće zaobilaženje problema da biste osmestili podrazumevanu kontrolnu tablu.</span><span class="sxs-lookup"><span data-stu-id="8e8c2-107">Use the following workaround to unset their default dashboard.</span></span>

1. <span data-ttu-id="8e8c2-108">Kreirajte novu ličnu tablu.</span><span class="sxs-lookup"><span data-stu-id="8e8c2-108">Create a new personal dashboard.</span></span>

2. <span data-ttu-id="8e8c2-109">Postavi tu novu kontrolnu tablu kao podrazumevanu vrednost korisnika.</span><span class="sxs-lookup"><span data-stu-id="8e8c2-109">Set that new dashboard as the user default.</span></span>

3. <span data-ttu-id="8e8c2-110">Izbrišite tu kontrolnu tablu.</span><span class="sxs-lookup"><span data-stu-id="8e8c2-110">Delete that dashboard.</span></span>

## <a name="the-dashboard-is-set-in-the-sitemap"></a><span data-ttu-id="8e8c2-111">Kontrolna tabla je postavljena na mapi sajta</span><span class="sxs-lookup"><span data-stu-id="8e8c2-111">The dashboard is set in the sitemap</span></span>

<span data-ttu-id="8e8c2-112">Možda ste odredili početnu kontrolnu tablu organizacije tako što ćete izabrati kontrolnu tablu i izabrati stavku "Postavi kao podrazumevano" u okviru "Prilagođavanje sistema".</span><span class="sxs-lookup"><span data-stu-id="8e8c2-112">You may have set an organization default dashboard by selecting a dashboard and choosing 'Set As Default' under 'Customize The System'.</span></span> <span data-ttu-id="8e8c2-113">Međutim, Kontrolna tabla koja je definisana u dizajneru "sajt" će imati prvenstvo iznad ove kontrolne table ako korisnik ima pristup.</span><span class="sxs-lookup"><span data-stu-id="8e8c2-113">But the dashboard defined in the sitemap designer will take precedence over this dashboard, if the user has access to it.</span></span>

<span data-ttu-id="8e8c2-114">Da bi korisnici videli kontrolnu tablu koju ste odredili kao podrazumevanu organizaciju, možete da:</span><span class="sxs-lookup"><span data-stu-id="8e8c2-114">To have users see the dashboard you've set as the organization default, you can either:</span></span>

* <span data-ttu-id="8e8c2-115">Podesite kontrolnu tablu na mapi sajta</span><span class="sxs-lookup"><span data-stu-id="8e8c2-115">Set that dashboard in the sitemap</span></span>

* <span data-ttu-id="8e8c2-116">Uklanjanje pristupa definisanoj kontrolnoj tabli za te korisnike</span><span class="sxs-lookup"><span data-stu-id="8e8c2-116">Remove access to the sitemap defined dashboard for those users</span></span>
