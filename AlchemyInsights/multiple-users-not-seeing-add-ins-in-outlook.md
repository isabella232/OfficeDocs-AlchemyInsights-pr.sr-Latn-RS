---
title: Više korisnika ne vidi programske dodatke u programu Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.openlocfilehash: 18d3fa535a88af18d8c4b02a5371d0a81c8d28c0
ms.sourcegitcommit: a05276bd623466ad211e1f8d9f0c616672dd3640
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 07/16/2020
ms.locfileid: "45198240"
---
# <a name="multiple-users-not-seeing-add-ins-in-outlook"></a><span data-ttu-id="409a9-102">Više korisnika ne vidi programske dodatke u programu Outlook</span><span class="sxs-lookup"><span data-stu-id="409a9-102">Multiple users not seeing add-ins in Outlook</span></span>

<span data-ttu-id="409a9-103">Ako testirate Outlook programske dodatke i ako se ništa ne prikaže, kao prvi korak za rešavanje problema, upotrebite funkciju " **Preuzmi konfiguraciju config** PowerShell" da biste proverili da li je parametar za _Appsforofficeenabled omogućen_ .</span><span class="sxs-lookup"><span data-stu-id="409a9-103">If you test Outlook add-ins and none show up, as a first troubleshooting step, use the **Get-OrganizationConfig** PowerShell cmdlet to query the _AppsForOfficeEnabled_ parameter.</span></span> <span data-ttu-id="409a9-104">Ako upit vraća vrednost **FALSE**, podesite ovaj parametar tako da koristi **Set-organizationconfig** cmdtime, tako da se programski dodaci **pojavljuju na očekivani** način.</span><span class="sxs-lookup"><span data-stu-id="409a9-104">If the query returns a value of **False**, set this parameter to **True** by using the **Set-OrganizationConfig** cmdlet, so add-ins appear as expected.</span></span>

<span data-ttu-id="409a9-105">Ne preporučujemo da parametar " _Appsforofficesa_ " je postavljen na **vrednost FALSE**.</span><span class="sxs-lookup"><span data-stu-id="409a9-105">We do not recommend that the _AppsForOfficeEnabled_ parameter is set to **False**.</span></span> <span data-ttu-id="409a9-106">Vrednost **FALSE** zamenjuje sve gorenavedene postavke administrativne i korisničke uloge i sprečava aktiviranje svih novih aplikacija u organizaciji.</span><span class="sxs-lookup"><span data-stu-id="409a9-106">A value of **False** overrides all of the above Administrative and User role settings and prevents any new apps from being activated by any user in the organization.</span></span>

<span data-ttu-id="409a9-107">Više informacija potražite u članku [Određivanje administratora i korisnika koji mogu da instaliraju i upravljaju programskim dodacima za Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins#user-roles).</span><span class="sxs-lookup"><span data-stu-id="409a9-107">For more information, see [Specify the administrators and users who can install and manage add-ins for Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins#user-roles).</span></span>