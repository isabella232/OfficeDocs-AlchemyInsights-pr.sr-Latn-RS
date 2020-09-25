---
title: 1490-rešavanje problema – otkazivanje
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1490"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: ff28f96d64ec14980e9a47b630246b394faf4610
ms.sourcegitcommit: fbe6925797cab0b38172386f1b059dc122e452a4
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/25/2020
ms.locfileid: "48277827"
---
# <a name="troubleshoot-content-search-errors"></a><span data-ttu-id="18c1d-102">Rešavanje problema sa pretraživanjem sadržaja</span><span class="sxs-lookup"><span data-stu-id="18c1d-102">Troubleshoot Content Search errors</span></span>

<span data-ttu-id="18c1d-103">Da li nailazite na probleme prilikom pretraživanja sadržaja ili neuspeha kada izvezete rezultate pretrage?</span><span class="sxs-lookup"><span data-stu-id="18c1d-103">Are you experiencing problems with Content Search or getting failures when you export search results?</span></span>

<span data-ttu-id="18c1d-104">Na primer, da li primate sledeće prilikom pokretanja pretraga?</span><span class="sxs-lookup"><span data-stu-id="18c1d-104">For example, are you receiving the following when running searches?</span></span>

- <span data-ttu-id="18c1d-105">CS008 ili CS012 greške</span><span class="sxs-lookup"><span data-stu-id="18c1d-105">CS008 or CS012 errors</span></span>

- <span data-ttu-id="18c1d-106">Greške na serveru/vremensko ograničenje</span><span class="sxs-lookup"><span data-stu-id="18c1d-106">Server busy/timeout errors</span></span>

- <span data-ttu-id="18c1d-107">Došlo je do greške prilikom aplikacije</span><span class="sxs-lookup"><span data-stu-id="18c1d-107">Application error occurred</span></span>

<span data-ttu-id="18c1d-108">Ili kada pretražujete ili izvozite rezultate iz velikog broja poštanskih sandučića (preko 100.000 poštanskih sandučića), da li dobijate greške izvoza?</span><span class="sxs-lookup"><span data-stu-id="18c1d-108">Or when searching or exporting results from a large number of mailboxes (over 100,000 mailboxes), are you getting export errors?</span></span>

<span data-ttu-id="18c1d-109">Za ove tipove grešaka ponovo pokušajte da pronađete lokacije sadržaja koje nisu uspele.</span><span class="sxs-lookup"><span data-stu-id="18c1d-109">For these types of errors, retry the search for the content locations that have failed.</span></span> <span data-ttu-id="18c1d-110">Više informacija potražite u  [članku ovaj članak](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) .</span><span class="sxs-lookup"><span data-stu-id="18c1d-110">See  [this article](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) for more information.</span></span>

<span data-ttu-id="18c1d-111">Ako izvozite više od 100K poštanskih sandučića, moraćete da koristite sledeće PowerShell za preuzimanje rezultata izvoza:  [izvoz rezultata iz više od 100k poštanskih sandučića](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).</span><span class="sxs-lookup"><span data-stu-id="18c1d-111">If you are exporting more than 100K mailboxes, you will need to use the following Powershell to download the Export results:  [Exporting results from more than 100K mailboxes](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).</span></span>
