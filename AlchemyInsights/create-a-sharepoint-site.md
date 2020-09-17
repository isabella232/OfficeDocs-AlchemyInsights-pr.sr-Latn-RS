---
title: Kreiranje SharePoint lokacije
ms.author: pebaum
author: pebaum
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ms.collection: Adm_O365
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "5200004"
- "3911416"
- "1386"
- "2303"
ms.assetid: e62b9f80-b017-42dc-9464-f4e32c19d6c9
ms.openlocfilehash: 5ebaa342ca9864bc31a9ef26eebcf42d96523871
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806953"
---
# <a name="create-a-sharepoint-site"></a><span data-ttu-id="65ea5-102">Kreiranje SharePoint lokacije</span><span class="sxs-lookup"><span data-stu-id="65ea5-102">Create a SharePoint site</span></span>

<span data-ttu-id="65ea5-103">Kreirajte ili Upravljajte lokacijama iz [aktivnih lokacija](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true) u SharePoint centru administracije.</span><span class="sxs-lookup"><span data-stu-id="65ea5-103">Create or manage sites from [Active Sites](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true) in the SharePoint Admin Center.</span></span> <span data-ttu-id="65ea5-104">Više informacija potražite u članku [Upravljanje lokacijama u novom SharePoint centru administracije](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="65ea5-104">For more info, see [Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span> 

## <a name="tips"></a><span data-ttu-id="65ea5-105">Nicama</span><span class="sxs-lookup"><span data-stu-id="65ea5-105">Tips:</span></span>

- <span data-ttu-id="65ea5-106">Ne **možete** da kreirate sajt sa istim URL adresom postojeće lokacije.</span><span class="sxs-lookup"><span data-stu-id="65ea5-106">You **cannot** create a site with the same URL of an existing site.</span></span> <span data-ttu-id="65ea5-107">Ako ste izbrisali lokaciju i želite da ponovo koristite URL, moguće je da izbrisana lokacija i dalje postoji u okviru [Izbrisane lokacije](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true).</span><span class="sxs-lookup"><span data-stu-id="65ea5-107">If you deleted a site and are wishing to re-use the URL, it's possible the deleted site still exists under [Deleted sites](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true).</span></span> <span data-ttu-id="65ea5-108">Lokacija treba trajno da bude izbrisana da biste ponovo koristili URL.</span><span class="sxs-lookup"><span data-stu-id="65ea5-108">The site will need to be permanently deleted to re-use the URL.</span></span> <span data-ttu-id="65ea5-109">Da biste u potpunosti uklonili veb sajt sa programom PowerShell, pogledajte primer cmdlet stavke za [Uklanjanje](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site)</span><span class="sxs-lookup"><span data-stu-id="65ea5-109">To completely remove a site with Powershell, see the [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet example.</span></span>
- <span data-ttu-id="65ea5-110">Neki korisnici možda neće moći da kreiraju sajt.</span><span class="sxs-lookup"><span data-stu-id="65ea5-110">Some users may not be able to create a site.</span></span> <span data-ttu-id="65ea5-111">[Pogledajte članak upravljanje kreiranjem lokacije u usluzi SharePoint online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="65ea5-111">[See Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span>
- <span data-ttu-id="65ea5-112">Moguće je da se lokacija pojavljuje u okviru **pravljenja** duže nego što je očekivano.</span><span class="sxs-lookup"><span data-stu-id="65ea5-112">It's possible the site appears stuck at **Creating** longer than expected.</span></span> <span data-ttu-id="65ea5-113">Ako je prošlo više od 24 časa od kada ste prvi put videli ovaj problem, prijavite karticu podrške.</span><span class="sxs-lookup"><span data-stu-id="65ea5-113">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="65ea5-114">U mnogim slučajevima, već radimo na rešenju.</span><span class="sxs-lookup"><span data-stu-id="65ea5-114">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="65ea5-115">Dajte nam najmanje 24 časa da biste dovršili rešenje.</span><span class="sxs-lookup"><span data-stu-id="65ea5-115">Please give us at least 24 hours to complete a solution.</span></span>
