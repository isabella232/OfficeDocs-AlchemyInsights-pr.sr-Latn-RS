---
title: Penzija nasleđenih alatki za eDiscovery
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
- "9001487"
- "3523"
ms.openlocfilehash: 2315c4c651a83f0ecc78c0171f32aba13bc93f8c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727797"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a><span data-ttu-id="f9219-102">Penzija nasleđenih alatki za eDiscovery</span><span class="sxs-lookup"><span data-stu-id="f9219-102">Retirement of Legacy eDiscovery Tools</span></span>

<span data-ttu-id="f9219-103">Kao rezultat nove i poboljšane funkcionalne funkcionalnosti u Microsoft 365 centru za usaglašenost, sledeće zastarele alatke za eDiscovery i zapovesti će se vratiti u narednih nekoliko meseci:</span><span class="sxs-lookup"><span data-stu-id="f9219-103">As a result of the new and improved eDiscovery functionality in Microsoft 365 Compliance center, the following legacy eDiscovery tools and commandlets will be retired in the coming months:</span></span>

- <span data-ttu-id="f9219-104">U [mestu eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) i [na](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) mestu se nalazi u Exchange centru administracije.</span><span class="sxs-lookup"><span data-stu-id="f9219-104">[In-Place eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) and [In-Place Holds](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) in the Exchange admin center.</span></span>

- <span data-ttu-id="f9219-105">Exchange online PowerShell cmdlet komande koji podržavaju funkcije ediscovery i na mestu će ga čuvati.</span><span class="sxs-lookup"><span data-stu-id="f9219-105">The Exchange Online PowerShell cmdlets that support In-Place eDiscovery and In-Place Holds.</span></span> <span data-ttu-id="f9219-106">(Ovi cmdlet zapisi kolektivno su identifikovani kao \*-mailboxsearch cmdlet komande.) To uključuje sledeće cmdlet sledeće:</span><span class="sxs-lookup"><span data-stu-id="f9219-106">(These cmdlets are collectively identified as \*-MailboxSearch cmdlets.) This includes the following cmdlets:</span></span>

    - [<span data-ttu-id="f9219-107">Novo-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="f9219-107">New-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [<span data-ttu-id="f9219-108">Start-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="f9219-108">Start-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [<span data-ttu-id="f9219-109">Stop-pošta Boxsearch</span><span class="sxs-lookup"><span data-stu-id="f9219-109">Stop-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [<span data-ttu-id="f9219-110">Scenofor-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="f9219-110">Set-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- <span data-ttu-id="f9219-111">[Pretraga – poštansko sanduče](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) cmdlet usluge Exchange online PowerShell.</span><span class="sxs-lookup"><span data-stu-id="f9219-111">The [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) cmdlet in Exchange Online PowerShell.</span></span>
- <span data-ttu-id="f9219-112">Sledeće operacije u usluzi Exchange Veb Services:</span><span class="sxs-lookup"><span data-stu-id="f9219-112">The following operations in the Exchange Web Services API:</span></span>
    - [<span data-ttu-id="f9219-113">Getsearchablemailbox</span><span class="sxs-lookup"><span data-stu-id="f9219-113">GetSearchableMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [<span data-ttu-id="f9219-114">Setholdone sandučići</span><span class="sxs-lookup"><span data-stu-id="f9219-114">SetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [<span data-ttu-id="f9219-115">Getholdone sandučići</span><span class="sxs-lookup"><span data-stu-id="f9219-115">GetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [<span data-ttu-id="f9219-116">Napredno eDiscovery v 1.0</span><span class="sxs-lookup"><span data-stu-id="f9219-116">Advanced eDiscovery v1.0</span></span>](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

<span data-ttu-id="f9219-117">**Vremenska osa za penziju**:</span><span class="sxs-lookup"><span data-stu-id="f9219-117">**Timeline for retirement**:</span></span>
- <span data-ttu-id="f9219-118">**1. jul, 2020** Više ne možete da kreirate nove pretrage i zadržavanje, ali možete da pokrećete, uređujete i brišete postojeće pretrage po sopstvenom riziku.</span><span class="sxs-lookup"><span data-stu-id="f9219-118">**July 1, 2020** You can no longer create new searches and holds, but you can run, edit, and delete existing searches at your own risk.</span></span> <span data-ttu-id="f9219-119">Microsoft Support više ne podržava na mjestu eDiscovery & čuva u EAC-u.</span><span class="sxs-lookup"><span data-stu-id="f9219-119">Microsoft Support no longer supports In-Place eDiscovery & Holds in the EAC.</span></span>
    
- <span data-ttu-id="f9219-120">**1 oktobar, 2020** Funkcija "eDiscovery &" u EAC-u biće postavljena u režimu samo za čitanje, tako da možete da uklonite samo postojeće pretrage i zadrške.</span><span class="sxs-lookup"><span data-stu-id="f9219-120">**October 1, 2020** In-Place eDiscovery & Holds functionality in the EAC will be placed in read-only mode, so you can only remove existing searches and holds.</span></span>

<span data-ttu-id="f9219-121">**Više informacija potražite u članku**:</span><span class="sxs-lookup"><span data-stu-id="f9219-121">**For more information, see**:</span></span>

 - [<span data-ttu-id="f9219-122">Migriranje zastarelih eDiscovery pretraga i držanje u Microsoft 365 centru za usaglašenost</span><span class="sxs-lookup"><span data-stu-id="f9219-122">Migrate legacy eDiscovery searches and holds to the Microsoft 365 compliance center</span></span>](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [<span data-ttu-id="f9219-123">Penzija nasleđenih alatki za eDiscovery</span><span class="sxs-lookup"><span data-stu-id="f9219-123">Retirement of legacy eDiscovery tools</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [<span data-ttu-id="f9219-124">Najčešća pitanja o otkrivanju na mestu koje se nalazi na sajtu i održavaju se na mestu</span><span class="sxs-lookup"><span data-stu-id="f9219-124">FAQs about In-Place eDiscovery and In-Place Holds</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



