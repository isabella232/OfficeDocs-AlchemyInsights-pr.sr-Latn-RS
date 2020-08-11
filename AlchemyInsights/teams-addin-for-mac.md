---
title: Programski dodatak za Mac za Mac
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/10/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6173"
- "9003233"
ms.openlocfilehash: 74bd424f71a59b80a91b960b815363668bee7036
ms.sourcegitcommit: 1361b2b37fd0201502a1a3547084961de284a3fc
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/11/2020
ms.locfileid: "46629855"
---
# <a name="teams-add-in-for-mac"></a><span data-ttu-id="a0661-102">Programski dodatak za Mac za Mac</span><span class="sxs-lookup"><span data-stu-id="a0661-102">Teams add-in for Mac</span></span>

<span data-ttu-id="a0661-103">Da biste rešili probleme sa programskim dodacima nestalih tima za Mac operativnog sistema, slijedite ove korake:</span><span class="sxs-lookup"><span data-stu-id="a0661-103">To troubleshoot a missing Teams add-in for Mac operating system users, follow these steps:</span></span>

<span data-ttu-id="a0661-104">**Prvi 1:** Ako imate lokalnu razmenu lokalnog programa (2016 CU3 ili noviju verziju), koristite alatku Test-HMA.ps1 da biste potvrdili da je hibridna savremena potvrda identiteta ispravno konfigurisana.</span><span class="sxs-lookup"><span data-stu-id="a0661-104">**Step 1:** If you have Hybrid Exchange On-Premises (2016 CU3 or later required), use the Test-HMA.ps1 tool to confirm that Hybrid Modern Authentication is correctly configured.</span></span> <span data-ttu-id="a0661-105">Više informacija potražite u članku [Provera valjanosti hibridne instalacije moderne potvrde identiteta za Outlook za iOS i Android](https://aka.ms/AA980zq).</span><span class="sxs-lookup"><span data-stu-id="a0661-105">For more info, see [Validating Hybrid Modern Authentication setup for Outlook for iOS and Android](https://aka.ms/AA980zq).</span></span>  

<span data-ttu-id="a0661-106">**Napomena** Koristite font UPN Adresa (na primer, [username@contoso.com](mailto:username@contoso.com)), a ne domen \ korisničko ime.</span><span class="sxs-lookup"><span data-stu-id="a0661-106">**Note** Use the UPN address format (for example, [username@contoso.com](mailto:username@contoso.com)), not domain\username.</span></span> <span data-ttu-id="a0661-107">Uradite to čak i za korisnike sa Exchange poštansko sanduče pošte.</span><span class="sxs-lookup"><span data-stu-id="a0661-107">Do this even for users with Exchange Online mailboxes.</span></span>

<span data-ttu-id="a0661-108">**2.2:** Neka korisnik ide na naloge **alatki**  >  **Accounts**... u programu Outlook za Mac i pronađite i izaberite nalog.</span><span class="sxs-lookup"><span data-stu-id="a0661-108">**Step 2:** Have the user go to **Tools** > **Accounts**... in Outlook for Mac, and find and select the account.</span></span> <span data-ttu-id="a0661-109">Potvrdite da je korisničko ime navedeno u UPN formatu (na primer, [username@contoso.com](mailto:username@contoso.com)).</span><span class="sxs-lookup"><span data-stu-id="a0661-109">Confirm the username listed is in UPN format (for example, [username@contoso.com](mailto:username@contoso.com)).</span></span>

<span data-ttu-id="a0661-110">**Treći broj:** Potvrdite da je korisnik licencirani Microsoft timovi.</span><span class="sxs-lookup"><span data-stu-id="a0661-110">**Step 3:** Confirm the user is a licensed Microsoft Teams user.</span></span> <span data-ttu-id="a0661-111">Korisnik mora da koristi pretplatu na Office 365 za Mac, verziju proizvoda 16,24 ili noviju verziju.</span><span class="sxs-lookup"><span data-stu-id="a0661-111">The user must be using the Office 365 for Mac subscription, product version 16.24 or later.</span></span>