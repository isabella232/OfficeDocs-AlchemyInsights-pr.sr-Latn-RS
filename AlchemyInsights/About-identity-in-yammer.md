---
title: O identitetu u mreži Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6039"
- "9003111"
ms.openlocfilehash: 2c4c2c836d18d2ab45e2368e778c793277b18aa0
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148304"
---
# <a name="about-identity-in-yammer"></a><span data-ttu-id="8c623-102">O identitetu u mreži Yammer</span><span class="sxs-lookup"><span data-stu-id="8c623-102">About identity in Yammer</span></span>

<span data-ttu-id="8c623-103">Preporučuje se da sve mreže preduzmu sledeće korake da biste izbegli probleme vezane za identitet:</span><span class="sxs-lookup"><span data-stu-id="8c623-103">It is recommended that all networks take the following steps to avoid identity-related issues:</span></span>

1. <span data-ttu-id="8c623-104">Nametni Office 365 identitet nakon što obezbedite Microsoft 365 naloge za korisnike u programu Azure oglasa da biste bili sigurni da se svi korisnici prijavljivanjem pomoću primarnog Microsoft 365 naloga.</span><span class="sxs-lookup"><span data-stu-id="8c623-104">Enforce Office 365 identity after provisioning Microsoft 365 accounts for users in Azure AD to ensure that all users sign in by using their primary Microsoft 365 account.</span></span> <span data-ttu-id="8c623-105">Više informacija potražite u članku [Primenjivanje Office 365 identiteta za korisnike mreže Yammer](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity).</span><span class="sxs-lookup"><span data-stu-id="8c623-105">For more info, see [Enforce Office 365 identity for Yammer users](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity).</span></span>
2. <span data-ttu-id="8c623-106">Konsolidovanje više mreža na mreži Yammer.</span><span class="sxs-lookup"><span data-stu-id="8c623-106">Consolidate multiple Yammer networks.</span></span> <span data-ttu-id="8c623-107">Zastarele konfiguracije mreže Yammer dozvoljavaju da više mreža na mreži Yammer bude povezano sa jednim tenkom.</span><span class="sxs-lookup"><span data-stu-id="8c623-107">Legacy Yammer configurations permit multiple Yammer networks to be connected to one tenant.</span></span> <span data-ttu-id="8c623-108">Više informacija potražite u članku [migracija mreže-konsolidovanje više mreža Yammer](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).</span><span class="sxs-lookup"><span data-stu-id="8c623-108">For more info, see [Network migration - Consolidate multiple Yammer networks](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).</span></span>
3. <span data-ttu-id="8c623-109">Opcionalno, primenite licencu za Yammer da biste blokirali korisnike sa mreže Yammer ako nemaju licencu.</span><span class="sxs-lookup"><span data-stu-id="8c623-109">Optionally, enforce licensing for Yammer to block users from Yammer if they don't have a license.</span></span> <span data-ttu-id="8c623-110">Više informacija potražite u članku [Upravljanje korisničkim licencama za Yammer u sistemu Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="8c623-110">For more info, see [Manage Yammer user licenses in Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).</span></span>
4. <span data-ttu-id="8c623-111">Na kraju, revizite listu korisnika za starije mreže Yammer i obustavite zastarele korisnike.</span><span class="sxs-lookup"><span data-stu-id="8c623-111">Finally, audit the user list for older Yammer networks and suspend legacy users.</span></span> <span data-ttu-id="8c623-112">Preporučuje se da obustavite (deaktivirate) korisnike umesto da ih izbrišete, jer je brisanje neopoziva.</span><span class="sxs-lookup"><span data-stu-id="8c623-112">It is recommended that you suspend (deactivate) users instead of deleting them, because deletion is irreversible.</span></span> <span data-ttu-id="8c623-113">Više informacija potražite u članku [nadgledanje korisnika Yammer na mrežama povezanim sa Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) i [Uklanjanje korisnika](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users).</span><span class="sxs-lookup"><span data-stu-id="8c623-113">For more info, see [Audit Yammer users in networks connected to Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) and [Remove users](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users).</span></span>

<span data-ttu-id="8c623-114">Ako konfigurišete Yammer pomoću ovih koraka, takođe ćete biti spremni da konfigurišete mrežu Yammer za osnovni režim za Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="8c623-114">By configuring Yammer using these steps, you'll also be ready to configure your Yammer network for Native Mode for Microsoft 365.</span></span> <span data-ttu-id="8c623-115">Više informacija potražite u članku [Konfigurisanje mreže Yammer za osnovni režim za Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode).</span><span class="sxs-lookup"><span data-stu-id="8c623-115">For more info, see [Configure your Yammer network for Native Mode for Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode).</span></span>