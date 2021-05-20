---
title: Teams programski dodatak za Mac
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/10/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6173"
- "6166"
- "9003233"
- "9002573"
ms.openlocfilehash: 45df4381688335f10f6699d8b5ff1aaafd6f7257
ms.sourcegitcommit: 730efbac8eec016b2b4f83f1b0e01e077f28c444
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 05/20/2021
ms.locfileid: "52582084"
---
# <a name="teams-add-in-for-mac"></a><span data-ttu-id="ae16e-102">Teams programski dodatak za Mac</span><span class="sxs-lookup"><span data-stu-id="ae16e-102">Teams add-in for Mac</span></span>

<span data-ttu-id="ae16e-103">Da biste rešili probleme sa Teams koji nedostaje za korisnike operativnog sistema Mac, pratite ove korake:</span><span class="sxs-lookup"><span data-stu-id="ae16e-103">To troubleshoot a missing Teams add-in for Mac operating system users, follow these steps:</span></span>

<span data-ttu-id="ae16e-104">**1. korak:** Ako imate Exchange hibridnu potvrdu identiteta (2016 CU3 ili kasnije obavezno), koristite alatku Test-HMA.ps1 da biste potvrdili da je hibridna moderna potvrda identiteta ispravno konfigurisana.</span><span class="sxs-lookup"><span data-stu-id="ae16e-104">**Step 1:** If you have Hybrid Exchange On-Premises (2016 CU3 or later required), use the Test-HMA.ps1 tool to confirm that Hybrid Modern Authentication is correctly configured.</span></span> <span data-ttu-id="ae16e-105">Više informacija potražite u članku [Provera valjanosti instalacije hibridne moderne potvrde identiteta za Outlook za iOS i Android.](https://aka.ms/TestHMAEAS)</span><span class="sxs-lookup"><span data-stu-id="ae16e-105">For more info, see [Validating Hybrid Modern Authentication setup for Outlook for iOS and Android](https://aka.ms/TestHMAEAS).</span></span>  

<span data-ttu-id="ae16e-106">**Napomišite** Koristite FORMAT UPN adrese (na primer [username@contoso.com](mailto:username@contoso.com)), ne domen\korisničko ime.</span><span class="sxs-lookup"><span data-stu-id="ae16e-106">**Note** Use the UPN address format (for example, [username@contoso.com](mailto:username@contoso.com)), not domain\username.</span></span> <span data-ttu-id="ae16e-107">Ovo radite čak i za korisnike sa Exchange Online poštanskim sandučićima.</span><span class="sxs-lookup"><span data-stu-id="ae16e-107">Do this even for users with Exchange Online mailboxes.</span></span>

<span data-ttu-id="ae16e-108">**2. korak:** Kada korisnik ode na **Alatke**  >  **Nalozi...** u Outlook za Mac, pronađite i izaberite nalog.</span><span class="sxs-lookup"><span data-stu-id="ae16e-108">**Step 2:** Have the user go to **Tools** > **Accounts**... in Outlook for Mac, and find and select the account.</span></span> <span data-ttu-id="ae16e-109">Potvrdite da je navedeno korisničko ime u UPN formatu (na [primer, username@contoso.com](mailto:username@contoso.com)).</span><span class="sxs-lookup"><span data-stu-id="ae16e-109">Confirm the username listed is in UPN format (for example, [username@contoso.com](mailto:username@contoso.com)).</span></span>

<span data-ttu-id="ae16e-110">**3. korak:** Potvrdite da je korisnik Microsoft Teams licenciran.</span><span class="sxs-lookup"><span data-stu-id="ae16e-110">**Step 3:** Confirm the user is a licensed Microsoft Teams user.</span></span> <span data-ttu-id="ae16e-111">Korisnik mora da koristi pretplatu na Office 365 Za Mac, verziju proizvoda 16.24 ili noviju.</span><span class="sxs-lookup"><span data-stu-id="ae16e-111">The user must be using the Office 365 for Mac subscription, product version 16.24 or later.</span></span>