---
title: Više korisnika preuzimanje greške zabrane pristupa pri dodavanju programskih dodataka u programu Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5892"
- "6700008"
ms.openlocfilehash: 624d880c535b7d8888b676ff23c774c6d138a75a
ms.sourcegitcommit: 07e56267dedfc4cec1143072c791670cbf81186b
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 07/24/2020
ms.locfileid: "45424173"
---
# <a name="multiple-users-get-access-denied-error-while-adding-add-ins-in-outlook"></a><span data-ttu-id="e5a27-102">Više korisnika preuzimanje greške zabrane pristupa pri dodavanju programskih dodataka u programu Outlook</span><span class="sxs-lookup"><span data-stu-id="e5a27-102">Multiple users get Access Denied error while adding add-ins in Outlook</span></span>

<span data-ttu-id="e5a27-103">Možete da navedete koje administratori u vašoj organizaciji imaju dozvolu da instaliraju i upravljaju programskim dodacima za Outlook.</span><span class="sxs-lookup"><span data-stu-id="e5a27-103">You can specify which administrators in your organization have permissions to install and manage add-ins for Outlook.</span></span> <span data-ttu-id="e5a27-104">Takođe možete odrediti koji korisnici u vašoj organizaciji imaju dozvolu da instaliraju i upravljaju programskim dodacima za svoje korišćenje.</span><span class="sxs-lookup"><span data-stu-id="e5a27-104">You can also specify which users in your organization have permission to install and manage add-ins for their own use.</span></span>

<span data-ttu-id="e5a27-105">Više informacija potražite u članku [Određivanje administratora i korisnika koji mogu da instaliraju i upravljaju programskim dodacima za Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).</span><span class="sxs-lookup"><span data-stu-id="e5a27-105">For details, see [Specify the administrators and users who can install and manage add-ins for Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins).</span></span>

<span data-ttu-id="e5a27-106">Da biste proverili da li ste uspešno dodelili dozvole za korisnika, zamenite <Role Name> ime uloge koju želite da proverite i pokrenite sledeću komandu u Exchange online PowerShell:</span><span class="sxs-lookup"><span data-stu-id="e5a27-106">To verify that you've successfully assigned permissions for a user, replace <Role Name> with the name of the role to verify, and run the following command in Exchange Online PowerShell:</span></span>

<span data-ttu-id="e5a27-107">Preuzimanje-uloga " <Role Name> "-GetEffectiveUsers</span><span class="sxs-lookup"><span data-stu-id="e5a27-107">Get-ManagementRoleAssignment -Role "<Role Name>" -GetEffectiveUsers</span></span>

<span data-ttu-id="e5a27-108">Ovaj primer vam pokazuje kako da proverite kome ste dodelili dozvole za instaliranje programskih dodataka iz Office prodavnice za organizaciju.</span><span class="sxs-lookup"><span data-stu-id="e5a27-108">This example shows you how to verify whom you've assigned permissions to install add-ins from the Office Store for the organization.</span></span>

<span data-ttu-id="e5a27-109">PowerShell</span><span class="sxs-lookup"><span data-stu-id="e5a27-109">PowerShell</span></span>

<span data-ttu-id="e5a27-110">-Uloga "aplikacije Marketplace org"-GetEffectiveUsers</span><span class="sxs-lookup"><span data-stu-id="e5a27-110">-Role "Org Marketplace Apps" -GetEffectiveUsers</span></span>

<span data-ttu-id="e5a27-111">U rezultatima, preuzmi i ponovo dodeli, Pregledajte stavke u koloni "efektivni korisnici".</span><span class="sxs-lookup"><span data-stu-id="e5a27-111">In the results, Get-ManagementRoleAssignment, review the entries in the Effective Users column.</span></span>

<span data-ttu-id="e5a27-112">Za detaljne informacije o sintaksi i parametrima pogledajte odeljak preuzimanje obaveštenja o [dodelju](https://docs.microsoft.com/powershell/module/exchange/get-managementroleassignment).</span><span class="sxs-lookup"><span data-stu-id="e5a27-112">For detailed syntax and parameter information, see [Get-ManagementRoleAssignment](https://docs.microsoft.com/powershell/module/exchange/get-managementroleassignment).</span></span>
 