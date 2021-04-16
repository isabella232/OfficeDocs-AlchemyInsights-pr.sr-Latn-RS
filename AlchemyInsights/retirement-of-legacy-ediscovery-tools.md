---
title: Retirement of Legacy eDiscovery Tools
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
- "9001487"
- "3523"
ms.openlocfilehash: 986c78f20e7b8c303c302913d63d817a56ce2896
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/15/2021
ms.locfileid: "51798563"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a><span data-ttu-id="65f45-102">Retirement of Legacy eDiscovery Tools</span><span class="sxs-lookup"><span data-stu-id="65f45-102">Retirement of Legacy eDiscovery Tools</span></span>

<span data-ttu-id="65f45-103">Kao rezultat nove i poboljšane funkcionalnosti e-discovery u Microsoft 365 centru za usaglašenost, sledeće zakupne alatke za e-discovery i komande će biti poništene u sledećim mesecima:</span><span class="sxs-lookup"><span data-stu-id="65f45-103">As a result of the new and improved eDiscovery functionality in Microsoft 365 Compliance center, the following legacy eDiscovery tools and commandlets will be retired in the coming months:</span></span>

- <span data-ttu-id="65f45-104">[Čuvanje čuvanja e-čuvanja](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) na mestu u Exchange centru adminitre. [](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds)</span><span class="sxs-lookup"><span data-stu-id="65f45-104">[In-Place eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) and [In-Place Holds](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) in the Exchange admin center.</span></span>

- <span data-ttu-id="65f45-105">Exchange Online PowerShell cmdlet In-Place e-discovery i čuvanje In-Place čuvanja podataka.</span><span class="sxs-lookup"><span data-stu-id="65f45-105">The Exchange Online PowerShell cmdlets that support In-Place eDiscovery and In-Place Holds.</span></span> <span data-ttu-id="65f45-106">(Ove cmdletlet menije su kolektivno identifikovane kao \*-MailboxSearch cmdlets.) To uključuje sledeće cmdlet mišove:</span><span class="sxs-lookup"><span data-stu-id="65f45-106">(These cmdlets are collectively identified as \*-MailboxSearch cmdlets.) This includes the following cmdlets:</span></span>

    - [<span data-ttu-id="65f45-107">New-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="65f45-107">New-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [<span data-ttu-id="65f45-108">Start-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="65f45-108">Start-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [<span data-ttu-id="65f45-109">Stop-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="65f45-109">Stop-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [<span data-ttu-id="65f45-110">Set-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="65f45-110">Set-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- <span data-ttu-id="65f45-111">Cmdlet [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) u programu Exchange Online PowerShell.</span><span class="sxs-lookup"><span data-stu-id="65f45-111">The [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) cmdlet in Exchange Online PowerShell.</span></span>
- <span data-ttu-id="65f45-112">Sledeće operacije u API-u Exchange veb usluga:</span><span class="sxs-lookup"><span data-stu-id="65f45-112">The following operations in the Exchange Web Services API:</span></span>
    - [<span data-ttu-id="65f45-113">GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="65f45-113">GetSearchableMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [<span data-ttu-id="65f45-114">SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="65f45-114">SetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [<span data-ttu-id="65f45-115">GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="65f45-115">GetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [<span data-ttu-id="65f45-116">Advanced eDiscovery v1.0</span><span class="sxs-lookup"><span data-stu-id="65f45-116">Advanced eDiscovery v1.0</span></span>](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

<span data-ttu-id="65f45-117">**Vremenska linija za penzionje:**</span><span class="sxs-lookup"><span data-stu-id="65f45-117">**Timeline for retirement**:</span></span>
- <span data-ttu-id="65f45-118">**1. jul 2020.** Više ne možete da kreirate nove pretrage i zadrške, ali možete da pokrećete, uređujete i brišete postojeće pretrage na sopstveni rizik.</span><span class="sxs-lookup"><span data-stu-id="65f45-118">**July 1, 2020** You can no longer create new searches and holds, but you can run, edit, and delete existing searches at your own risk.</span></span> <span data-ttu-id="65f45-119">Microsoft podrška više ne podržava čuvanje In-Place e-& u EAC-u.</span><span class="sxs-lookup"><span data-stu-id="65f45-119">Microsoft Support no longer supports In-Place eDiscovery & Holds in the EAC.</span></span>
    
- <span data-ttu-id="65f45-120">**1. oktobar 2020.** In-Place funkcionalnost & čuvanja čuvanja u EAC-u biće postavljena u režim samo za čitanje, tako da možete da uklonite samo postojeće pretrage i zadrške.</span><span class="sxs-lookup"><span data-stu-id="65f45-120">**October 1, 2020** In-Place eDiscovery & Holds functionality in the EAC will be placed in read-only mode, so you can only remove existing searches and holds.</span></span>

<span data-ttu-id="65f45-121">**Dodatne informacije potražite u:**</span><span class="sxs-lookup"><span data-stu-id="65f45-121">**For more information, see**:</span></span>

 - [<span data-ttu-id="65f45-122">Migrirane zakasnele pretrage i zadrške u Microsoft 365 centru za usaglašenost</span><span class="sxs-lookup"><span data-stu-id="65f45-122">Migrate legacy eDiscovery searches and holds to the Microsoft 365 compliance center</span></span>](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [<span data-ttu-id="65f45-123">Retirement of legacy eDiscovery tools</span><span class="sxs-lookup"><span data-stu-id="65f45-123">Retirement of legacy eDiscovery tools</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [<span data-ttu-id="65f45-124">FaQs about In-Place e-discovery and In-Place Holds</span><span class="sxs-lookup"><span data-stu-id="65f45-124">FAQs about In-Place eDiscovery and In-Place Holds</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



