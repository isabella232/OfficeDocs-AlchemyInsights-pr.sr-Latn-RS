---
title: Upravljanje kontrolisanim identitetom koji je dodelio korisnik
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8211"
- "9003230"
ms.openlocfilehash: a44cb484b6d89e6d5f67b2900c38dde3610b0e23
ms.sourcegitcommit: 23e778f7414e5f1a98cc786146fe76d622b458bc
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 02/10/2021
ms.locfileid: "50177775"
---
# <a name="manage-a-user-assigned-managed-identity"></a><span data-ttu-id="eb550-102">Upravljanje kontrolisanim identitetom koji je dodelio korisnik</span><span class="sxs-lookup"><span data-stu-id="eb550-102">Manage a user-assigned managed identity</span></span>

<span data-ttu-id="eb550-103">Upravljanje kontrolisanim korisničkim identitetom uključuje:</span><span class="sxs-lookup"><span data-stu-id="eb550-103">The management of a user-assigned managed identity involves:</span></span>

- <span data-ttu-id="eb550-104">Dodeljivanje uloga korisniku dodeljenom kontrolisanom identitetu</span><span class="sxs-lookup"><span data-stu-id="eb550-104">Assigning roles to a user-assigned managed identity</span></span>
- <span data-ttu-id="eb550-105">Brisanje korisničkog kontrolisanog identiteta koji je dodelio korisnik</span><span class="sxs-lookup"><span data-stu-id="eb550-105">Deleting a user-assigned managed identity</span></span>
- <span data-ttu-id="eb550-106">Navođenje korisnog kontrolisanog identiteta korisnika</span><span class="sxs-lookup"><span data-stu-id="eb550-106">Listing a user-assigned managed identity</span></span>

<span data-ttu-id="eb550-107">Više informacija o gorenavedenim zadacima potražite u sledećim člancima:</span><span class="sxs-lookup"><span data-stu-id="eb550-107">For more information on the tasks mentioned above, see the following articles:</span></span>

- <span data-ttu-id="eb550-108">[Kako da kreirate korisnički kontrolisani identitet koji je dodeljen](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/how-to-manage-ua-identity-portal) korisniku – za dodeljivanje uloga korisniku dodeljenom identitetu</span><span class="sxs-lookup"><span data-stu-id="eb550-108">[How to create a user-assigned managed identity](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/how-to-manage-ua-identity-portal) - for assigning roles to a user-assigned managed identity</span></span>
- <span data-ttu-id="eb550-109">[Kako se briše kontrolisani identitet koji se dodeljuje korisniku](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/how-to-manage-ua-identity-portal) – za brisanje korisnikog identiteta dodeljenog korisniku</span><span class="sxs-lookup"><span data-stu-id="eb550-109">[How to delete a user-assigned managed identity](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/how-to-manage-ua-identity-portal) - for deleting a user-assigned managed identity</span></span>
- <span data-ttu-id="eb550-110">[Kako se navodi korisnički kontrolisani identitet koji je dodelio korisnik](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/how-to-manage-ua-identity-portal) – za listu popisanog kontrolisanog identiteta koji je dodelio korisnik</span><span class="sxs-lookup"><span data-stu-id="eb550-110">[How to list a user-assigned managed identity](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/how-to-manage-ua-identity-portal) - for listing a user-assigned managed identity</span></span>

> [!NOTE]
> <span data-ttu-id="eb550-111">Proverite da li imate dodelu uloge **saradnika saradnika** .</span><span class="sxs-lookup"><span data-stu-id="eb550-111">Verify whether you have the **Managed Identity Contributor** role assignment.</span></span> <span data-ttu-id="eb550-112">Taj zadatak je obavezan za kreiranje/brisanje korisnik koji se dodeljuje.</span><span class="sxs-lookup"><span data-stu-id="eb550-112">That role assignment is required for creating/deleting user-assigned managed identities.</span></span>
