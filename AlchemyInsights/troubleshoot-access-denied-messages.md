---
title: Rešavanje problema sa pristupom "zabranjen pristup"
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 3550081a12379f73725253214a2c2d44974ab740
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47690797"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="a9c1d-102">Rešavanje problema sa pristupom "zabranjen pristup"</span><span class="sxs-lookup"><span data-stu-id="a9c1d-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="a9c1d-103">Ako je neko dobio poruku "pristup je odbijen" u deljenoj fascikli u sistemu SharePoint, administrator kolekcije lokacija je možda omogućio "sistem zatvaranja korisnika lokacije sa ograničenom pristupom".</span><span class="sxs-lookup"><span data-stu-id="a9c1d-103">If someone got an "Access Denied" message to a shared folder in SharePoint, the site collection administrator might have enabled "Limited-access user permission lockdown mode."</span></span> <span data-ttu-id="a9c1d-104">Da biste isključili ovu opciju:</span><span class="sxs-lookup"><span data-stu-id="a9c1d-104">To turn this off:</span></span> 
  
1. <span data-ttu-id="a9c1d-105">Pronađite lokaciju, kliknite na ikonu postavke, a zatim izaberite stavku **Postavke sajta**.</span><span class="sxs-lookup"><span data-stu-id="a9c1d-105">Browse to the site, click the Settings icon, and then click **Site Settings**.</span></span>
    
2. <span data-ttu-id="a9c1d-106">U okviru **Administracija kolekcije lokacija**izaberite stavku **funkcije kolekcije lokacija**.</span><span class="sxs-lookup"><span data-stu-id="a9c1d-106">Under **Site Collection Administration**, click **Site collection features**.</span></span>
    
3. <span data-ttu-id="a9c1d-107">Pored **ograničenog režima zatvaranja dozvole za ograničenje korisnika**, kliknite na dugme **Deaktiviraj**.</span><span class="sxs-lookup"><span data-stu-id="a9c1d-107">Next to **Limited-access user permission lockdown mode**, click **Deactivate**.</span></span>
    
<span data-ttu-id="a9c1d-108">Poruka "pristup odbijen" takođe može da se pojavi za deljene fascikle ako je lokacija lokacija za objavljivanje.</span><span class="sxs-lookup"><span data-stu-id="a9c1d-108">An Access Denied message can also occur for shared folders if the site is a publishing site.</span></span> <span data-ttu-id="a9c1d-109">Informacije potražite u članku [zabranjen pristup prilikom pristupanja deljenoj fascikli](https://go.microsoft.com/fwlink/?linkid=2004317).</span><span class="sxs-lookup"><span data-stu-id="a9c1d-109">For info, see [Access Denied when accessing a shared folder](https://go.microsoft.com/fwlink/?linkid=2004317).</span></span>
  
<span data-ttu-id="a9c1d-110">Ako neko ima poruku "pristup nije dozvoljen" kada pokušate da prikažete zahteve za pristup, korisnik mora da se doda kao administrator kolekcije lokacija ili član grupe vlasnika za sajt.</span><span class="sxs-lookup"><span data-stu-id="a9c1d-110">If a someone got an "Access Denied" message when trying to view access requests, the user needs to be added as either a site collection administrator or a member of the Owners group for the site.</span></span> <span data-ttu-id="a9c1d-111">Više informacija potražite u članku [zabranjen pristup listi zahteva za pristup](https://go.microsoft.com/fwlink/?linkid=2004220).</span><span class="sxs-lookup"><span data-stu-id="a9c1d-111">For more info, see [Access Denied to Access Requests list](https://go.microsoft.com/fwlink/?linkid=2004220).</span></span>
  
<span data-ttu-id="a9c1d-112">Ako je korisnik dobio poruku "pristup je odbijen" nakon što su uklonjene iz aktivnog direktorijuma i ponovo dodata, pogledajte članak [zabranjen pristup kada se korisnički nalog sinhronizuje sa Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span><span class="sxs-lookup"><span data-stu-id="a9c1d-112">If a user got an "Access Denied" message after they were removed from Active Directory on-premises and then added back, see [Access Denied when a user account is synced to Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span></span>
  

