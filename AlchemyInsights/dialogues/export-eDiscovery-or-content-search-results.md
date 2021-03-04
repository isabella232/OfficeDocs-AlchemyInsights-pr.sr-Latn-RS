---
title: Izvoz rezultata pretrage eDiscovery/otkrivanja sadržaja
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3200003"
- "7221"
ms.openlocfilehash: b93377a33eebc7899041b684449e46caedb04415
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/04/2021
ms.locfileid: "50429971"
---
# <a name="export-ediscoverycontent-search-results"></a><span data-ttu-id="b422a-102">Izvoz rezultata pretrage eDiscovery/otkrivanja sadržaja</span><span class="sxs-lookup"><span data-stu-id="b422a-102">Export eDiscovery/Content Search results</span></span>

<span data-ttu-id="b422a-103">Možda ćete morati da izvezete rezultate pretrage u PST datoteku (iz e-pošte) ili u izvorne Office dokumente (iz sistema SharePoint i usluge OneDrive for Business sites).</span><span class="sxs-lookup"><span data-stu-id="b422a-103">You may need to export your search results to a PST file (from email) or to native Office documents (from SharePoint and OneDrive for Business sites).</span></span> <span data-ttu-id="b422a-104">Ako je tako, uradite sledeće:</span><span class="sxs-lookup"><span data-stu-id="b422a-104">If so, do the following:</span></span>

- <span data-ttu-id="b422a-105">Uverite se da je nalogu dodeljen odgovarajući pristup za izvoz.</span><span class="sxs-lookup"><span data-stu-id="b422a-105">Make sure your account is assigned the proper permissions to export.</span></span> <span data-ttu-id="b422a-106">Više informacija potražite u članku [dodeljivanje dozvole za eDiscovery](https://go.microsoft.com/fwlink/?linkid=2102406).</span><span class="sxs-lookup"><span data-stu-id="b422a-106">For more info, see [Assign eDiscovery permission](https://go.microsoft.com/fwlink/?linkid=2102406).</span></span>
- <span data-ttu-id="b422a-107">Uverite se da je računar ispunio sve [preduslove](https://docs.microsoft.com/office365/securitycompliance/export-search-results#before-you-begin).</span><span class="sxs-lookup"><span data-stu-id="b422a-107">Make sure your computer has met all [prerequisites](https://docs.microsoft.com/office365/securitycompliance/export-search-results#before-you-begin).</span></span> <span data-ttu-id="b422a-108">Nisu podržani svi pregledači, kao što je Chrome.</span><span class="sxs-lookup"><span data-stu-id="b422a-108">Not all browsers are supported, such as Chrome.</span></span>
- <span data-ttu-id="b422a-109">Da biste izvezli iz pretrage sadržaja: a.</span><span class="sxs-lookup"><span data-stu-id="b422a-109">To export from a Content Search: a.</span></span> <span data-ttu-id="b422a-110">Idite u [Centar za bezbednost & bezbednosti](https://protection.office.com/contentsearch) i kliknite na dugme **Pretraži**, a zatim izaberite stavku **Pretraga sadržaja**.</span><span class="sxs-lookup"><span data-stu-id="b422a-110">Go to the [Security & Compliance Center](https://protection.office.com/contentsearch) and click **Search**, and then select **Content search**.</span></span> <span data-ttu-id="b422a-111">Na stranici **Pretraga sadržaja** izaberite sačuvanu pretragu.</span><span class="sxs-lookup"><span data-stu-id="b422a-111">On the **Content search** page, select a saved search.</span></span>
    <span data-ttu-id="b422a-112">-.</span><span class="sxs-lookup"><span data-stu-id="b422a-112">b.</span></span> <span data-ttu-id="b422a-113">U oknu detalji, u okviru **Izvezi rezultate na računar**, izaberite stavku **Započni izvoz**.</span><span class="sxs-lookup"><span data-stu-id="b422a-113">On the Details pane, under **Export results to a computer**, select **Start export**.</span></span> <span data-ttu-id="b422a-114">Ako izvozite više od 100K poštanskih sandučića, moraćete da koristite PowerShell da biste preuzeli rezultate izvoza.</span><span class="sxs-lookup"><span data-stu-id="b422a-114">If you're exporting more than 100K mailboxes, you'll need to use PowerShell to download the export results.</span></span> <span data-ttu-id="b422a-115">Više informacija potražite u članku [izvoz rezultata iz više od 100K poštanskih sandučića](https://go.microsoft.com/fwlink/?linkid=2143861).</span><span class="sxs-lookup"><span data-stu-id="b422a-115">For more info, see [Exporting results from more than 100K mailboxes](https://go.microsoft.com/fwlink/?linkid=2143861).</span></span>

<span data-ttu-id="b422a-116">Da biste saznali više, pogledajte članak [izvoz rezultata pretrage sadržaja](https://go.microsoft.com/fwlink/?linkid=2102118).</span><span class="sxs-lookup"><span data-stu-id="b422a-116">To learn more, see [Export Content Search Results](https://go.microsoft.com/fwlink/?linkid=2102118).</span></span>