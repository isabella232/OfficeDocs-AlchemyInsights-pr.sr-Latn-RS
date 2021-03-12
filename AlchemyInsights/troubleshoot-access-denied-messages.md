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
ms.openlocfilehash: 6c8ad84123fb58b73b9c378592ce970997893ea2
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/10/2021
ms.locfileid: "50704908"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="6777e-102">Rešavanje problema sa pristupom "zabranjen pristup"</span><span class="sxs-lookup"><span data-stu-id="6777e-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="6777e-103">Ako je neko dobio poruku "pristup je odbijen" u deljenoj fascikli u sistemu SharePoint, administrator kolekcije lokacija je možda omogućio "sistem zatvaranja korisnika lokacije sa ograničenom pristupom".</span><span class="sxs-lookup"><span data-stu-id="6777e-103">If someone got an "Access Denied" message to a shared folder in SharePoint, the site collection administrator might have enabled "Limited-access user permission lockdown mode."</span></span> <span data-ttu-id="6777e-104">Da biste isključili ovu opciju:</span><span class="sxs-lookup"><span data-stu-id="6777e-104">To turn this off:</span></span> 
  
1. <span data-ttu-id="6777e-105">Pronađite lokaciju, kliknite na ikonu postavke, a zatim izaberite stavku **Postavke sajta**.</span><span class="sxs-lookup"><span data-stu-id="6777e-105">Browse to the site, click the Settings icon, and then click **Site Settings**.</span></span>
    
2. <span data-ttu-id="6777e-106">U okviru **Administracija kolekcije lokacija** izaberite stavku **funkcije kolekcije lokacija**.</span><span class="sxs-lookup"><span data-stu-id="6777e-106">Under **Site Collection Administration**, click **Site collection features**.</span></span>
    
3. <span data-ttu-id="6777e-107">Pored **ograničenog režima zatvaranja dozvole za ograničenje korisnika**, kliknite na dugme **Deaktiviraj**.</span><span class="sxs-lookup"><span data-stu-id="6777e-107">Next to **Limited-access user permission lockdown mode**, click **Deactivate**.</span></span>
    
<span data-ttu-id="6777e-108">Poruka "pristup odbijen" takođe može da se pojavi za deljene fascikle ako je lokacija lokacija za objavljivanje.</span><span class="sxs-lookup"><span data-stu-id="6777e-108">An Access Denied message can also occur for shared folders if the site is a publishing site.</span></span> <span data-ttu-id="6777e-109">Informacije potražite u članku [zabranjen pristup prilikom pristupanja deljenoj fascikli](https://answers.microsoft.com/windows/forum/windows_7-files/access-denied-to-share-folder/79fae49d-cddf-4845-8ac8-c141884d85fb).</span><span class="sxs-lookup"><span data-stu-id="6777e-109">For info, see [Access Denied when accessing a shared folder](https://answers.microsoft.com/windows/forum/windows_7-files/access-denied-to-share-folder/79fae49d-cddf-4845-8ac8-c141884d85fb).</span></span>
  
<span data-ttu-id="6777e-110">Ako neko ima poruku "pristup nije dozvoljen" kada pokušate da prikažete zahteve za pristup, korisnik mora da se doda kao administrator kolekcije lokacija ili član grupe vlasnika za sajt.</span><span class="sxs-lookup"><span data-stu-id="6777e-110">If a someone got an "Access Denied" message when trying to view access requests, the user needs to be added as either a site collection administrator or a member of the Owners group for the site.</span></span> <span data-ttu-id="6777e-111">Više informacija potražite u članku [zabranjen pristup listi zahteva za pristup](https://go.microsoft.com/fwlink/?linkid=2004220).</span><span class="sxs-lookup"><span data-stu-id="6777e-111">For more info, see [Access Denied to Access Requests list](https://go.microsoft.com/fwlink/?linkid=2004220).</span></span>
  
<span data-ttu-id="6777e-112">Ako je korisnik dobio poruku "pristup je odbijen" nakon što su uklonjene iz aktivnog direktorijuma i ponovo dodata, pogledajte članak [zabranjen pristup kada se korisnički nalog sinhronizuje sa Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span><span class="sxs-lookup"><span data-stu-id="6777e-112">If a user got an "Access Denied" message after they were removed from Active Directory on-premises and then added back, see [Access Denied when a user account is synced to Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span></span>
  

