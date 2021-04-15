---
title: Teams 4c7 greška
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3472"
- "9001211"
ms.openlocfilehash: 51f2aa936e803b63bcbdf73b89959cd3a1757751
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/15/2021
ms.locfileid: "51786683"
---
# <a name="4c7-error-in-microsoft-teams"></a><span data-ttu-id="f3264-102">4c7 greška u aplikaciji Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="f3264-102">4c7 error in Microsoft Teams</span></span>

<span data-ttu-id="f3264-103">Do ove greške dolazi zato što Microsoft Teams zahteva potvrdu identiteta obrasca.</span><span class="sxs-lookup"><span data-stu-id="f3264-103">This error occurs because Microsoft Teams requires Forms Authentication.</span></span> <span data-ttu-id="f3264-104">Kada primenite Active Directory usluge za ukidanje (AD FS), potvrda identiteta obrazaca nije podrazumevano omogućena za intranet.</span><span class="sxs-lookup"><span data-stu-id="f3264-104">When you deploy Active Directory Federation Services (AD FS), Forms Authentication is not enabled for the intranet by default.</span></span> <span data-ttu-id="f3264-105">Ako Windows integrisana potvrda identiteta ne uspe, bićete upitani da se prijavite pomoću potvrde identiteta obrasca.</span><span class="sxs-lookup"><span data-stu-id="f3264-105">If Windows Integrated Authentication fails, you are prompted to sign in by using Forms Authentication.</span></span>

<span data-ttu-id="f3264-106">Da biste rešili ovaj problem, omogućite potvrdu identiteta obrasca pomoću proširenja konzole AD FS Microsoft Management Console (MMC) na računaru koji ima lokalnu kopiju usluge Active Directory.</span><span class="sxs-lookup"><span data-stu-id="f3264-106">To resolve this issue, enable Forms Authentication by using the AD FS Microsoft Management Console (MMC) snap-in on the computer that has the local copy of Active Directory.</span></span> <span data-ttu-id="f3264-107">Da biste to uradio, sledite ove korake:</span><span class="sxs-lookup"><span data-stu-id="f3264-107">To do this, follow these steps:</span></span> 

1. <span data-ttu-id="f3264-108">U oknu za navigaciju potražite smernice **za potvrdu identiteta.**</span><span class="sxs-lookup"><span data-stu-id="f3264-108">In the navigation pane, browse to **Authentication Policies**.</span></span>
2. <span data-ttu-id="f3264-109">U **okviru Radnje** u oknu sa detaljima, izaberite stavku **Uredi globalnu primarnu potvrdu identiteta.**</span><span class="sxs-lookup"><span data-stu-id="f3264-109">Under **Actions** in the details pane, select **Edit Global Primary Authentication**.</span></span>
3. <span data-ttu-id="f3264-110">Na kartici **Intranet** izaberite stavku **Potvrda identiteta obrazaca**.</span><span class="sxs-lookup"><span data-stu-id="f3264-110">On the **Intranet** tab, select **Forms Authentication**.</span></span>
4. <span data-ttu-id="f3264-111">Izaberite **stavku U** redu (ili **Primeni**).</span><span class="sxs-lookup"><span data-stu-id="f3264-111">Select **OK** (or **Apply**).</span></span>