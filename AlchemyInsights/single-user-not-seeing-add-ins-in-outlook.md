---
title: Dodatni korisnici ne vide programske dodatke u programu Outlook
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
ms.openlocfilehash: 1f547c3f593b3256bd44f518aacbc36ed1c4c848
ms.sourcegitcommit: a05276bd623466ad211e1f8d9f0c616672dd3640
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 07/16/2020
ms.locfileid: "45198218"
---
# <a name="single-user-not-seeing-add-ins-in-outlook"></a><span data-ttu-id="ddcb5-102">Dodatni korisnici ne vide programske dodatke u programu Outlook</span><span class="sxs-lookup"><span data-stu-id="ddcb5-102">Single user not seeing add-ins in Outlook</span></span>

<span data-ttu-id="ddcb5-103">Korisnik može biti deo uloge koja nema tačan parametar Appsforofficeovog parametra.</span><span class="sxs-lookup"><span data-stu-id="ddcb5-103">The user might be part of a role that doesn’t have the correct AppsForOfficeEnabled parameter.</span></span> <span data-ttu-id="ddcb5-104">Pokreni ovu cmdme da biste saznali da li je ispravna uloga povezana sa korisnikom:</span><span class="sxs-lookup"><span data-stu-id="ddcb5-104">Run this cmdlet to find out if the correct role is associated with the user:</span></span>

<span data-ttu-id="ddcb5-105">Preuzmite-"Roledodeljenog" user@domain.com-delegiranje $false | Format-tabal-uloga auto-a, Roledodeljenog Neename</span><span class="sxs-lookup"><span data-stu-id="ddcb5-105">Get-ManagementRoleAssignment -RoleAssignee user@domain.com -Delegating $false | Format-Table -Auto Role,RoleAssigneeName,RoleAssigneeType</span></span>

<span data-ttu-id="ddcb5-106">Više informacija potražite u članku [Određivanje administratora i korisnika koji mogu da instaliraju i upravljaju programskim dodacima za Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).</span><span class="sxs-lookup"><span data-stu-id="ddcb5-106">For more info, see [Specify the administrators and users who can install and manage add-ins for Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).</span></span>
