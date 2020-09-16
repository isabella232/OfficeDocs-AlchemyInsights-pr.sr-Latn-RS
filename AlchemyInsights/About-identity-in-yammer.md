---
title: O identitetu u usluzi Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6039"
- "9003111"
ms.openlocfilehash: f417117acac4c3040932fc0a35e5d0b1c3709cd5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664184"
---
# <a name="about-identity-in-yammer"></a><span data-ttu-id="022f7-102">O identitetu u usluzi Yammer</span><span class="sxs-lookup"><span data-stu-id="022f7-102">About identity in Yammer</span></span>

<span data-ttu-id="022f7-103">Preporučuje se da sve mreže preduzmu sledeće korake da bi se izbegli problemi u vezi sa identitetom:</span><span class="sxs-lookup"><span data-stu-id="022f7-103">It is recommended that all networks take the following steps to avoid identity-related issues:</span></span>

1. <span data-ttu-id="022f7-104">Nametanje Office 365 identiteta nakon obezbeđivanja Microsoft 365 naloga za korisnike u Azure AD da biste se uverili da se svi korisnici prijave pomoću primarnog Microsoft 365 naloga.</span><span class="sxs-lookup"><span data-stu-id="022f7-104">Enforce Office 365 identity after provisioning Microsoft 365 accounts for users in Azure AD to ensure that all users sign in by using their primary Microsoft 365 account.</span></span> <span data-ttu-id="022f7-105">Više informacija potražite u članku [nametanje primene Office 365 identiteta za Yammer korisnike](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity).</span><span class="sxs-lookup"><span data-stu-id="022f7-105">For more info, see [Enforce Office 365 identity for Yammer users](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity).</span></span>
2. <span data-ttu-id="022f7-106">Konsolidovanje više Yammer mreža.</span><span class="sxs-lookup"><span data-stu-id="022f7-106">Consolidate multiple Yammer networks.</span></span> <span data-ttu-id="022f7-107">Zastarele konfiguracije usluge Yammer dozvoljava da se više Yammer mreža poveže sa jednim zakupcem.</span><span class="sxs-lookup"><span data-stu-id="022f7-107">Legacy Yammer configurations permit multiple Yammer networks to be connected to one tenant.</span></span> <span data-ttu-id="022f7-108">Više informacija potražite u članku [migracija na mreži – konsolidacija više Yammer mreža](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).</span><span class="sxs-lookup"><span data-stu-id="022f7-108">For more info, see [Network migration - Consolidate multiple Yammer networks](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).</span></span>
3. <span data-ttu-id="022f7-109">Opcionalno, nametanje licenciranja za Yammer da blokirate korisnike iz usluge Yammer ako nemaju licencu.</span><span class="sxs-lookup"><span data-stu-id="022f7-109">Optionally, enforce licensing for Yammer to block users from Yammer if they don't have a license.</span></span> <span data-ttu-id="022f7-110">Više informacija potražite u članku [Upravljanje korisničkim licencama usluge Yammer u sistemu Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="022f7-110">For more info, see [Manage Yammer user licenses in Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).</span></span>
4. <span data-ttu-id="022f7-111">Konačno, nadzor liste korisnika za starije Yammer mreže i suspenduje zastarele korisnike.</span><span class="sxs-lookup"><span data-stu-id="022f7-111">Finally, audit the user list for older Yammer networks and suspend legacy users.</span></span> <span data-ttu-id="022f7-112">Preporučuje se da obustavite (Deaktivirajte) korisnike umesto da ih brišete zato što je brisanje neopoziva.</span><span class="sxs-lookup"><span data-stu-id="022f7-112">It is recommended that you suspend (deactivate) users instead of deleting them, because deletion is irreversible.</span></span> <span data-ttu-id="022f7-113">Više informacija potražite u članku [nadgledanje Yammer korisnika u mrežama povezanim sa sistemom Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) i [uklanjanjem korisnika](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users).</span><span class="sxs-lookup"><span data-stu-id="022f7-113">For more info, see [Audit Yammer users in networks connected to Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) and [Remove users](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users).</span></span>

<span data-ttu-id="022f7-114">Konfigurisanjem Yammer pomoću ovih koraka takođe ćete biti spremni da konfigurišete Yammer mrežu za izvorni režim za Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="022f7-114">By configuring Yammer using these steps, you'll also be ready to configure your Yammer network for Native Mode for Microsoft 365.</span></span> <span data-ttu-id="022f7-115">Više informacija potražite u članku [Konfigurisanje Yammer mreže za izvorni režim za Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode).</span><span class="sxs-lookup"><span data-stu-id="022f7-115">For more info, see [Configure your Yammer network for Native Mode for Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode).</span></span>