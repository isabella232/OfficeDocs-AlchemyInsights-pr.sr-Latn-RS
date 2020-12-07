---
title: 'Uloge u RBAC-u '
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003230"
- "7265"
ms.openlocfilehash: 7c4c9d1a76f395dfb2f831d555199b76c354ca57
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 12/04/2020
ms.locfileid: "49583951"
---
# <a name="rbac-rules"></a><span data-ttu-id="b2dd7-102">Pravila za RBAC</span><span class="sxs-lookup"><span data-stu-id="b2dd7-102">RBAC rules</span></span>

<span data-ttu-id="b2dd7-103">Ako dobijete grešku sa dozvolom:</span><span class="sxs-lookup"><span data-stu-id="b2dd7-103">If you get the permission error:</span></span> 

- <span data-ttu-id="b2dd7-104">**Klijent sa ID-om objekta nema ovlaštenja da izvršava radnju iznad opsega (kôd: autorizacija nije uspelo)**: kada pokušate da kreirate resurs, uverite se da ste trenutno prijavljeni sa korisnikom koji ima dozvolu za upisivanje u resurs na izabranom opsegu.</span><span class="sxs-lookup"><span data-stu-id="b2dd7-104">**The client with object id does not have authorization to perform action over scope (code: AuthorizationFailed)**: when you try to create a resource, check that you are currently signed in with a user that is assigned a role that has write permission to the resource at the selected scope.</span></span> <span data-ttu-id="b2dd7-105">Na primer, da biste upravljali virtuelnim mašinama u grupi resursa, trebalo bi da imate ulogu [saradnika virtualnog mašinskog](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor) programa u grupi resursa (ili nadređenom opsegu).</span><span class="sxs-lookup"><span data-stu-id="b2dd7-105">For example, to manage virtual machines in a resource group, you should have the [Virtual Machine Contributor](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor) role on the resource group (or parent scope).</span></span> <span data-ttu-id="b2dd7-106">Listu dozvola za svaku ugrađenu ulogu potražite [u članku ugrađene uloge za Azure resurse](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="b2dd7-106">For a list of the permissions for each built-in role, see [Built-in roles for Azure resources](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
- <span data-ttu-id="b2dd7-107">Nemate **dozvolu da kreirate zahtev za podršku**: kada pokušate da kreirate ili ažurirate karte za podršku, uverite se da ste trenutno prijavljeni sa korisnikom kojem je dodeljena uloga koja ima Microsoft. support/support karte/pišite dozvole, kao što je [doprinos podrške](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor).</span><span class="sxs-lookup"><span data-stu-id="b2dd7-107">**You don't have permission to create a support request**: when you try to create or update a support ticket, check that you are currently signed in with a user that is assigned a role that has the Microsoft.Support/supportTickets/write permission, such as [Support Request Contributor](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor).</span></span>
- <span data-ttu-id="b2dd7-108">**Ne možete da kreirate više dodeljenih uloga (kôd: Roleromentograniиenje premašivanja)**: kada pokušate da dodelite ulogu, pokušajte da smanjite broj dodeljivanja uloga tako što dodeljujete uloge grupama.</span><span class="sxs-lookup"><span data-stu-id="b2dd7-108">**No more role assignments can be created (code: RoleAssignmentLimitExceeded)**: when you try to assign a role, try to reduce the number of role assignments by assigning roles to groups instead.</span></span> <span data-ttu-id="b2dd7-109">Azure podržava do **2000** dodeljivanja uloga po pretplati.</span><span class="sxs-lookup"><span data-stu-id="b2dd7-109">Azure supports up to **2000** role assignments per subscription.</span></span>

<span data-ttu-id="b2dd7-110">Više detalja o Azure RBAC ulogama potražite u članku [AZURE rbac uloge](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="b2dd7-110">For more details on Azure RBAC roles, see [Azure RBAC roles](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
