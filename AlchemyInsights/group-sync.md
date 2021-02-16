---
title: Sinhronizacija grupe
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8304"
- "9003234"
ms.openlocfilehash: 52c19b6dcc79968150a188b389c5481c122f7945
ms.sourcegitcommit: 6900c2b7208ca51a9873dfc2e00be6f66cb25e3c
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 02/15/2021
ms.locfileid: "50256787"
---
# <a name="group-sync"></a><span data-ttu-id="af058-102">Sinhronizacija grupe</span><span class="sxs-lookup"><span data-stu-id="af058-102">Group sync</span></span>

<span data-ttu-id="af058-103">Ovaj članak pruža uputstva za sinhronizaciju grupe.</span><span class="sxs-lookup"><span data-stu-id="af058-103">This article provides guidance on group synchronization.</span></span>

1. <span data-ttu-id="af058-104">Ako globalni administrator ili vlasnik grupe ne mogu da izmene svojstva grupe ili dodaju članove ili dodeljuju vlasnike na Azure portal, uverite se da je izvor autoriteta za grupu administrator Azure Active Directory (Azure AD) za globalnog administratora ili vlasnika grupe koji će izmeniti grupu.</span><span class="sxs-lookup"><span data-stu-id="af058-104">If a global admin or group owner is not able to modify group properties or add members or assign owners in the Azure portal, ensure the source of the authority for the group is Azure Active Directory (Azure AD) for the global admin or group owner to modify the group.</span></span>
2. <span data-ttu-id="af058-105">Pre nego što pokušate da izbrišete sinhronizovanu grupu u usluzi Azure AD, uverite se da ste [izbrisali sve dodeljene licence](https://docs.microsoft.com/azure/active-directory/enterprise-users/licensing-group-advanced) da biste izbegli greške.</span><span class="sxs-lookup"><span data-stu-id="af058-105">Before attempting to delete a synced group in Azure AD, ensure you have [deleted all assigned licenses](https://docs.microsoft.com/azure/active-directory/enterprise-users/licensing-group-advanced) to avoid errors.</span></span>

<span data-ttu-id="af058-106">Da biste razumeli kako da sinhronizujete korisnike, grupe i kontakte, pogledajte [AZURE AD Connect Sync](https://docs.microsoft.com/azure/active-directory/hybrid/concept-azure-ad-connect-sync-user-and-contacts)i prateći [sinhronizaciju lokalno grupe do Azure pomoću usluge Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/whatis-hybrid-identity?WT.mc_id=Portal-Microsoft_Azure_Support) za sinhronizaciju sa OPERATIVNIM sistemom grupe koristeći AD Connect.</span><span class="sxs-lookup"><span data-stu-id="af058-106">For understanding how to sync users, groups and contacts, see [Azure AD Connect Sync](https://docs.microsoft.com/azure/active-directory/hybrid/concept-azure-ad-connect-sync-user-and-contacts), and follow [Syncing an on-premises group to Azure using Azure AD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/whatis-hybrid-identity?WT.mc_id=Portal-Microsoft_Azure_Support) to sync on-perm groups using AD connect.</span></span>

<span data-ttu-id="af058-107">Izvršite ovaj vodič za [Rešavanje problema tokom sinhronizacije](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sync-errors) da biste rešili probleme sa uobičajenim greškama tokom sinhronizacije.</span><span class="sxs-lookup"><span data-stu-id="af058-107">Follow this guide [Troubleshooting Errors during synchronization](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sync-errors) to troubleshoot common errors during synchronization.</span></span>

