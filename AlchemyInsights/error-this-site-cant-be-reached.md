---
title: Nije moguće postići grešku prilikom pokušaja pristupa SharePoint lokaciji iz pregledača ili timova
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/11/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9005378"
- "9266"
ms.openlocfilehash: 451544fb85522e0eececc9274825805699685ee9
ms.sourcegitcommit: 186281d0b87d67f041c127d4334faa937da9a48a
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/11/2021
ms.locfileid: "50747040"
---
# <a name="this-site-cant-be-reached-error-when-trying-to-access-sharepoint-site-from-browser-or-teams"></a><span data-ttu-id="0d1ba-102">Greška "nije moguće postići" kada pokušate da pristupite SharePoint lokaciji iz pregledača ili timova</span><span class="sxs-lookup"><span data-stu-id="0d1ba-102">“This site can’t be reached” error when trying to access SharePoint site from browser or Teams</span></span>

<span data-ttu-id="0d1ba-103">Korisnici mogu dobiti grešku "Ova lokacija ne može da se dostigne" kada pokušam da pristupim SharePoint lokaciji iz pregledača ili timova.</span><span class="sxs-lookup"><span data-stu-id="0d1ba-103">Users might receive "This site can't be reached" error when trying to access SharePoint site from browser or Teams.</span></span> 

<span data-ttu-id="0d1ba-104">Da biste rešili ovaj problem:</span><span class="sxs-lookup"><span data-stu-id="0d1ba-104">To resolve this issue:</span></span> 

1. <span data-ttu-id="0d1ba-105">Potvrdite da li se matična stranica nalazi u korpi za otpatke ili u korpi za otpatke druge faze i vratite stranicu.</span><span class="sxs-lookup"><span data-stu-id="0d1ba-105">Check if the home page is in Recycle bin or second-stage recycle bin and restore the page.</span></span>

<span data-ttu-id="0d1ba-106">**Uzorak direktne URL adrese za reciklažu**: https://contoso.sharepoint.com/sites/siteA/_layouts/15/RecycleBin.aspx</span><span class="sxs-lookup"><span data-stu-id="0d1ba-106">**Sample direct URL to recycle bin**: https://contoso.sharepoint.com/sites/siteA/_layouts/15/RecycleBin.aspx</span></span>

1. <span data-ttu-id="0d1ba-107">Ako je matična stranica trajno uklonjena iz korpe za otpatke, kreirajte stranicu "Nova lokacija" iz biblioteke stranica lokacije i neka bude matična stranica.</span><span class="sxs-lookup"><span data-stu-id="0d1ba-107">If the home page is permanently removed from the recycle bin, create a new site page from the Site Pages library and make it a homepage.</span></span> 

<span data-ttu-id="0d1ba-108">**Direktna probna adresa**: https://contoso.sharepoint.com/sites/siteA/_layouts/15/RecycleBin.aspx</span><span class="sxs-lookup"><span data-stu-id="0d1ba-108">**Sample direct URL**: https://contoso.sharepoint.com/sites/siteA/_layouts/15/RecycleBin.aspx</span></span>