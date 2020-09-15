---
title: Pristup uslugama penzija
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 943066d5ac76c0630554ee724bbab9a94086fae4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47698696"
---
# <a name="access-services-retirement"></a><span data-ttu-id="fb645-102">Pristup uslugama penzija</span><span class="sxs-lookup"><span data-stu-id="fb645-102">Access services retirement</span></span>

<span data-ttu-id="fb645-103">Kao što smo se prvobitno najavili u MC97576, u martu 2017 i nastavili smo da komuniciramo u prethodnim godišnjim uslugama za pristup.</span><span class="sxs-lookup"><span data-stu-id="fb645-103">As we originally announced in MC97576, in March 2017, and continued to communicate over the past year Access Services are being retired.</span></span> <span data-ttu-id="fb645-104">Sledeća faza u ovom procesu je uklanjanje Access Veb baza podataka koje koriste SharePoint liste kao osnovno skladište podataka.</span><span class="sxs-lookup"><span data-stu-id="fb645-104">The next phase in this process will be the removal of Access Web Databases that use SharePoint lists as their underlying data storage.</span></span>

<span data-ttu-id="fb645-105">**Kako to utiče na mene?**</span><span class="sxs-lookup"><span data-stu-id="fb645-105">**How does this affect me?**</span></span>

<span data-ttu-id="fb645-106">Počevši od juna 2019, Zaustavićemo kreiranje novih Access baza podataka u sistemu SharePoint Online i isključiti uslugu i sve preostale aplikacije do aprila 2020.</span><span class="sxs-lookup"><span data-stu-id="fb645-106">Starting June 2019, we will stop creation of new Access databases in SharePoint Online and shut down the service and any remaining apps by April 2020.</span></span>

<span data-ttu-id="fb645-107">**Šta treba da uradim da bih se pripremio za ovu promenu?**</span><span class="sxs-lookup"><span data-stu-id="fb645-107">**What do I need to do to prepare for this change?**</span></span>

<span data-ttu-id="fb645-108">Podstićemo vas da kreirate prelaz plan za Access Veb baze podataka organizacije.</span><span class="sxs-lookup"><span data-stu-id="fb645-108">We encourage you to create a transition plan for your organization's Access web databases.</span></span> <span data-ttu-id="fb645-109">Administratori mogu da koriste [SharePoint Access skener aplikacija](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) da bi nabavili zalihe Access aplikacija koje lokacije koriste.</span><span class="sxs-lookup"><span data-stu-id="fb645-109">Admins can use the [SharePoint Access app scanner](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) to obtain an inventory of the Access apps that sites are using.</span></span>

<span data-ttu-id="fb645-110">Postoji nekoliko načina za migraciju podataka iz Veb baze podataka:</span><span class="sxs-lookup"><span data-stu-id="fb645-110">There are several ways to migrate Access web databases data:</span></span>

- <span data-ttu-id="fb645-111">Uvoz u lokalnu Access bazu podataka (. ACCDB) ili Excel datoteku.</span><span class="sxs-lookup"><span data-stu-id="fb645-111">Importing to a local Access database (.ACCDB) or to an Excel file.</span></span>
- <span data-ttu-id="fb645-112">Preporučujemo da istražimo Microsoft PowerApps kao alternativnu platformu za kreiranje nekodova Business Solutions za Veb i mobilne uređaje.</span><span class="sxs-lookup"><span data-stu-id="fb645-112">We also recommend exploring Microsoft PowerApps as an alternative platform to create no-code business solutions for web and mobile devices.</span></span>