---
title: MC210173 – Novi prilagođeni obrazac zastarevanja funkcije SharePoint Designer programa
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002886"
- "5508"
- "9000127"
- "5507"
ms.openlocfilehash: 5be1ac4c8a4044adbc7d37c32ba7b3cb67c6cc25
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/15/2021
ms.locfileid: "51831820"
---
# <a name="mc210173---sharepoint-designer-new-custom-form-feature-deprecation"></a><span data-ttu-id="86329-102">MC210173 – Novi prilagođeni obrazac zastarevanja funkcije SharePoint Designer programa</span><span class="sxs-lookup"><span data-stu-id="86329-102">MC210173 - SharePoint Designer new custom Form feature deprecation</span></span>

<span data-ttu-id="86329-103">Identifikovali smo problem koji utiče na funkcionalnost SharePoint Designer programa za [kreiranje prilagođenih obrazaca](https://support.microsoft.com/en-us/office/create-a-custom-list-form-using-sharepoint-designer-917d8fdb-ee00-4441-adb3-a94612d1d105?ui=en-us&rs=en-us&ad=us#bm2) unutar usluge SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="86329-103">We’ve identified an issue affecting SharePoint Designer functionality for [creating custom Forms](https://support.microsoft.com/en-us/office/create-a-custom-list-form-using-sharepoint-designer-917d8fdb-ee00-4441-adb3-a94612d1d105?ui=en-us&rs=en-us&ad=us#bm2) within SharePoint Online.</span></span> <span data-ttu-id="86329-104">Nakon pažljivog ispitivanja, utvrdili smo da ne postoji poznata ispravka za ovaj problem i odlučili smo da onemogućimo prilagođenu funkciju izrade obrasca koja će važiti od 3:00 UTC u subotu, 25. aprila 2020.</span><span class="sxs-lookup"><span data-stu-id="86329-104">After careful examination, we’ve determined that there is no known fix for this issue and have elected to disable the custom Form creation feature effective as of 3:00 AM UTC on Saturday, April 25, 2020.</span></span> <span data-ttu-id="86329-105">Ova promena ne utiče na mogućnost uređivanja prethodno stvorenih obrasca ili drugih postojećih funkcija u SharePoint Online dizajneru.</span><span class="sxs-lookup"><span data-stu-id="86329-105">This change does not impact the ability to edit previously created Forms or other existing features in SharePoint Online Designer.</span></span>

<span data-ttu-id="86329-106">Nakon što je ova promena izvršena, korisnici su možda dobili grešku: „Nije moguće sačuvati promene na listi servera“ prilikom kreiranja novih obrazaca.</span><span class="sxs-lookup"><span data-stu-id="86329-106">After this change was made, users may have received the error: "Could not save the list changes to the server," when creating new Forms.</span></span>

<span data-ttu-id="86329-107">Korisnici koji su prethodno koristili SharePoint Designer za kreiranje prilagođenih obrasca umesto toga mogu da iskoriste [PowerApps](https://docs.microsoft.com/powerapps/maker/canvas-apps/customize-list-form) u tu svrhu.</span><span class="sxs-lookup"><span data-stu-id="86329-107">Users who have previously leveraged SharePoint Designer to create custom Forms are instead able to utilize [PowerApps](https://docs.microsoft.com/powerapps/maker/canvas-apps/customize-list-form) for this purpose.</span></span>

<span data-ttu-id="86329-108">PowerApps je jednostavan i moćan alat koji omogućava korisnicima koji rade u SharePoint Online modernom iskustvu da kreiraju i uređuju prilagođene obrasce za SharePoint liste i biblioteke dokumenata direktno iz prozora pregledača.</span><span class="sxs-lookup"><span data-stu-id="86329-108">PowerApps is an easy and powerful tool that allows users operating in the SharePoint Online Modern experience to create and edit custom Forms for SharePoint lists and document libraries right from a browser window.</span></span> <span data-ttu-id="86329-109">PowerApps ne zahteva tradicionalno znanje kodiranja ili bilo koje dodatno preuzimanje aplikacija kao što je InfoPath.</span><span class="sxs-lookup"><span data-stu-id="86329-109">PowerApps does not require traditional coding knowledge or any additional app downloads such as InfoPath.</span></span>

<span data-ttu-id="86329-110">**Napomena**: SharePoint Online klasični korisnici moraće da se privremeno prebace na moderno iskustvo da bi pristupili PowerApps i koriste PowerApps. Međutim, svim prilagođenim obrascima koji su kreirani u PowerApps mogu da pristupe korisnici SharePoint Online klasičnog iskustva.</span><span class="sxs-lookup"><span data-stu-id="86329-110">**Note**: SharePoint Online Classic users will need to temporarily switch to the Modern experience to access and utilize PowerApps; though, all custom Forms created in PowerApps are accessible by SharePoint Online Classic experience users.</span></span>
