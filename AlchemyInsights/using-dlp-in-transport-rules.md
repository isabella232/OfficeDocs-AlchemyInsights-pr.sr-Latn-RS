---
title: Korišćenje DLP u pravilima za prenos
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002635"
- "5153"
ms.openlocfilehash: e512b36b34c5fc4931fb0f796790ee4b01c6443c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/15/2021
ms.locfileid: "51827230"
---
# <a name="using-dlp-in-transport-rules"></a><span data-ttu-id="7b755-102">Korišćenje DLP u pravilima za prenos</span><span class="sxs-lookup"><span data-stu-id="7b755-102">Using DLP in transport rules</span></span>

<span data-ttu-id="7b755-103">Da biste integrisali Sprečavanje gubitka podataka (DLP) u postojeći prenos, koristite uslov „**Ako poruka sadrži... Osetljive informacije**” u postavci pravila za prenos.</span><span class="sxs-lookup"><span data-stu-id="7b755-103">To integrate Data Loss Prevention (DLP) into an existing transport, use the condition "**If the message contains...Sensitive Information**" in the Transport rule setting.</span></span>

<span data-ttu-id="7b755-104">**Za više detalja pogledajte:**</span><span class="sxs-lookup"><span data-stu-id="7b755-104">**For more details, see:**</span></span>

- <span data-ttu-id="7b755-105">Integrisani DLP tipovi osetljivih informacija u pravilima za prenos: [Integrisanje pravila za osetljive informacije](https://docs.microsoft.com/exchange/security-and-compliance/data-loss-prevention/integrate-sensitive-information-rules).</span><span class="sxs-lookup"><span data-stu-id="7b755-105">Integrated DLP sensitive information types in transport rules: [Integrate Sensitive Information Rules](https://docs.microsoft.com/exchange/security-and-compliance/data-loss-prevention/integrate-sensitive-information-rules).</span></span>

<span data-ttu-id="7b755-106">Korišćenjem režima testiranja možete takođe da testirate pravilo sa ili bez test smernice.</span><span class="sxs-lookup"><span data-stu-id="7b755-106">You can also test the rule with or without policy test using Test Mode on the rule.</span></span>  <span data-ttu-id="7b755-107">Trebalo bi da sačekate 30 minuta nakon kreiranja pravila pre nego što ga testirate.</span><span class="sxs-lookup"><span data-stu-id="7b755-107">You should wait 30 mins after creating the rule before testing it.</span></span>

- <span data-ttu-id="7b755-108">Pogledajte [Testiranje tokova pošte/pravila prenosa](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules)</span><span class="sxs-lookup"><span data-stu-id="7b755-108">See [Test Mail Flow/Transport rules](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules)</span></span>

<span data-ttu-id="7b755-109">**Napomena**: Ako pokušavate da primenite nove DLP smernice sa pravilima prenosa u EAC-u, koristite [DLP smernice u centru za bezbednost i usaglašenost](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies?view=o365-worldwide) umesto toga.</span><span class="sxs-lookup"><span data-stu-id="7b755-109">**Note**: If you are trying to implement a new DLP policy with transport rules in the EAC, use [DLP Policies in the Security and Compliance center](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies?view=o365-worldwide) instead.</span></span>
