---
title: Greška tima 4c7
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3472"
- "9001211"
ms.openlocfilehash: 08494b461a24eba8999a5edb99c89af7b17db9b3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700217"
---
# <a name="4c7-error-in-microsoft-teams"></a><span data-ttu-id="f3263-102">Greška 4c7 u Microsoft timovima</span><span class="sxs-lookup"><span data-stu-id="f3263-102">4c7 error in Microsoft Teams</span></span>

<span data-ttu-id="f3263-103">Do ove greške dolazi zato što Microsoft zahteva potvrdu identiteta.</span><span class="sxs-lookup"><span data-stu-id="f3263-103">This error occurs because Microsoft Teams requires Forms Authentication.</span></span> <span data-ttu-id="f3263-104">Kada primenite usluge usluge za Active Directory (AD FS), potvrda identiteta obrazaca se podrazumevano ne omogućava za intranet.</span><span class="sxs-lookup"><span data-stu-id="f3263-104">When you deploy Active Directory Federation Services (AD FS), Forms Authentication is not enabled for the intranet by default.</span></span> <span data-ttu-id="f3263-105">Ako Integrisana Windows potvrda identiteta ne uspe, bićete upitani da se prijavite pomoću potvrde identiteta obrazaca.</span><span class="sxs-lookup"><span data-stu-id="f3263-105">If Windows Integrated Authentication fails, you are prompted to sign in by using Forms Authentication.</span></span>

<span data-ttu-id="f3263-106">Da biste rešili ovaj problem, omogućite proveru identiteta obrazaca tako što ćete koristiti proširenje programskog dodatka AD FS Microsoft Management Console (MMC) na računaru koji ima lokalnu kopiju aktivnog direktorijuma.</span><span class="sxs-lookup"><span data-stu-id="f3263-106">To resolve this issue, enable Forms Authentication by using the AD FS Microsoft Management Console (MMC) snap-in on the computer that has the local copy of Active Directory.</span></span> <span data-ttu-id="f3263-107">Da biste to uradili, pratite ove korake:</span><span class="sxs-lookup"><span data-stu-id="f3263-107">To do this, follow these steps:</span></span> 

1. <span data-ttu-id="f3263-108">U oknu za navigaciju potražite smernice za **potvrdu identiteta**.</span><span class="sxs-lookup"><span data-stu-id="f3263-108">In the navigation pane, browse to **Authentication Policies**.</span></span>
2. <span data-ttu-id="f3263-109">U okviru **Radnje** u oknu detalji izaberite stavku **Uredi globalnu primarnu potvrdu identiteta**.</span><span class="sxs-lookup"><span data-stu-id="f3263-109">Under **Actions** in the details pane, select **Edit Global Primary Authentication**.</span></span>
3. <span data-ttu-id="f3263-110">Na kartici **intranet** izaberite stavku **potvrda identiteta obrazaca**.</span><span class="sxs-lookup"><span data-stu-id="f3263-110">On the **Intranet** tab, select **Forms Authentication**.</span></span>
4. <span data-ttu-id="f3263-111">Izaberite stavku **u redu** (ili se **primenjuje**).</span><span class="sxs-lookup"><span data-stu-id="f3263-111">Select **OK** (or **Apply**).</span></span>