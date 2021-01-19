---
title: Rešavanje problema sa vlasnikom
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7815"
- "9004358"
ms.openlocfilehash: 914d5682a403197a8569bb75fda8a77449f485f6
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901279"
---
# <a name="troubleshoot-owner-issues"></a><span data-ttu-id="af689-102">Rešavanje problema sa vlasnikom</span><span class="sxs-lookup"><span data-stu-id="af689-102">Troubleshoot owner issues</span></span>

<span data-ttu-id="af689-103">Da biste rešili probleme sa vlasnikom, obavite sledeće korake:</span><span class="sxs-lookup"><span data-stu-id="af689-103">To troubleshoot owner-related issues, perform the following steps:</span></span>

1. <span data-ttu-id="af689-104">[Dodajte ili promenite Azure administratorske administratore](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-accessmanagement-managing-group-owners): Azure Active Directory (AZURE AD) grupe su u vlasništvu i upravljaju ih vlasnici grupe.</span><span class="sxs-lookup"><span data-stu-id="af689-104">[Add or change Azure subscription administrators](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-accessmanagement-managing-group-owners): Azure Active Directory (Azure AD) groups are owned and managed by group owners.</span></span> <span data-ttu-id="af689-105">Vlasnici grupe mogu biti korisnici ili direktori usluga i mogu upravljati grupom, uključujući članstvo.</span><span class="sxs-lookup"><span data-stu-id="af689-105">Group owners can be users or service principals, and are able to manage the group, including membership.</span></span> <span data-ttu-id="af689-106">Samo postojeći vlasnici grupa ili administratori grupe mogu da dodele vlasnike grupa.</span><span class="sxs-lookup"><span data-stu-id="af689-106">Only existing group owners or group-managing administrators can assign group owners.</span></span> <span data-ttu-id="af689-107">Vlasnici grupe ne moraju da budu članovi grupe.</span><span class="sxs-lookup"><span data-stu-id="af689-107">Group owners aren't required to be members of the group.</span></span>
2. <span data-ttu-id="af689-108">[Dodavanje ili promena Azure administratora pretplate](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator): ovaj članak opisuje kako da dodate ili promenite ulogu administratora za korisnika pomoću AZURE rbac na nivou pretplate.</span><span class="sxs-lookup"><span data-stu-id="af689-108">[Add or change Azure subscription administrators](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator): This article describes how to add or change the administrator role for a user using Azure RBAC at the subscription scope.</span></span>
3. <span data-ttu-id="af689-109">Koristite PowerShell da biste dodali vlasnika grupe ili vlasnika aplikacije.</span><span class="sxs-lookup"><span data-stu-id="af689-109">Use PowerShell to add a group owner or an application owner.</span></span>
