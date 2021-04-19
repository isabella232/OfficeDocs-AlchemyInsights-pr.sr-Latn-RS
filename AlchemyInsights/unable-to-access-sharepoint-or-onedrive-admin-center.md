---
title: Nije moguće pristupiti SharePoint ili OneDrive centru aktivnosti
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
- "9001459"
- "5638"
ms.openlocfilehash: 7ba4a9c6995c03dd21e0e1aa387e407d41a08fb1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/15/2021
ms.locfileid: "51824449"
---
# <a name="unable-to-access-sharepoint-or-onedrive-admin-center"></a><span data-ttu-id="b206c-102">Nije moguće pristupiti SharePoint ili OneDrive centru aktivnosti</span><span class="sxs-lookup"><span data-stu-id="b206c-102">Unable to access SharePoint or OneDrive admin center</span></span>

- <span data-ttu-id="b206c-103">Ako je lokacija SharePoint ili OneDrive centra administratora nedostupna ili je nedostupna, možda postoji privremeni problem sa uslugom gde korisnici nailaziju na povremena odlaganja ili greške u navigaciji prilikom pristupa SharePoint lokacijama ili OneDrive sadržaju.</span><span class="sxs-lookup"><span data-stu-id="b206c-103">If your SharePoint or OneDrive Admin center site is inaccessible or unavailable, there may be a temporary service issue where users experience intermittent delays or navigation errors when accessing SharePoint sites or OneDrive content.</span></span> <span data-ttu-id="b206c-104">Proverite [kontrolnu tablu Za zdravstveno stanje usluge](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) da biste videli da li to utiče na vašu organizaciju.</span><span class="sxs-lookup"><span data-stu-id="b206c-104">Check the [Service health dashboard](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>

- <span data-ttu-id="b206c-105">Globalnim i SharePointadministartima treba dodeliti SharePoint licencu.</span><span class="sxs-lookup"><span data-stu-id="b206c-105">Global and SharePoint admins need to be assigned a SharePoint license.</span></span> <span data-ttu-id="b206c-106">Novi kreirani nalozi koji su upravo dodeljeni sa ulogom SharePoint licence ili ulogom administarcionog može imati problema sa pristupom programu SharePoint, kao što su "pristup je odbijen" ili "nije pronađen korisnik".</span><span class="sxs-lookup"><span data-stu-id="b206c-106">Newly created accounts just assigned with a SharePoint License or Admin role might experience issues accessing SharePoint, like "access denied" or "user not found."</span></span> <span data-ttu-id="b206c-107">Sačekajte najmanje 24 časa da se sinhronizacija dovrši u svim sistemima.</span><span class="sxs-lookup"><span data-stu-id="b206c-107">Please give at least 24 hours for sync to complete across our systems.</span></span> <span data-ttu-id="b206c-108">Razumemo da 24 časa mogu izgledati kao dugo vreme.</span><span class="sxs-lookup"><span data-stu-id="b206c-108">We understand that 24 hours may seem like a long time.</span></span> <span data-ttu-id="b206c-109">U mnogim slučajevima već radimo na rešenju.</span><span class="sxs-lookup"><span data-stu-id="b206c-109">In many cases, we're already working on a solution.</span></span>

- <span data-ttu-id="b206c-110">Korisnici privileged Identity Management ([PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-add-role-to-user?tabs=new)) mogu da dobiju pristup odbijen ako je veoma mali prozor vremena dozvoljenog pristupa. Pogledajte pristup zabranjen [PIM nalozima.](https://docs.microsoft.com/sharepoint/troubleshoot/administration/access-denied-to-pim-user-accounts)</span><span class="sxs-lookup"><span data-stu-id="b206c-110">Privileged Identity Management ([PIM](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-how-to-add-role-to-user?tabs=new))  users may receive access denied if allowed access time window is very small, see  [Access denied to PIM accounts](https://docs.microsoft.com/sharepoint/troubleshoot/administration/access-denied-to-pim-user-accounts).</span></span>