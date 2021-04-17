---
title: Mikro kašnjenja ili ograničavanje u usluzi Exchange Online PowerShell
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
- "3500011"
- "5106"
ms.openlocfilehash: 680df9e6e2404ff6b60b17d6ac88e202e9a7bb25
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830047"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a><span data-ttu-id="b857e-102">Mikro kašnjenja ili ograničavanje u usluzi Exchange Online PowerShell</span><span class="sxs-lookup"><span data-stu-id="b857e-102">Micro delays or throttling in Exchange Online PowerShell</span></span>

<span data-ttu-id="b857e-103">Možda ćete videti upozorenja „Primenjeno je mikro kašnjenje“ ili kašnjenja kada pokrenete skripte ili cmdlet komande u usluzi Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="b857e-103">You might see "Micro delay applied" warnings or delays when you run scripts and cmdlets in Exchange Online.</span></span> <span data-ttu-id="b857e-104">Evo dva predloga koja se odnose na ovo:</span><span class="sxs-lookup"><span data-stu-id="b857e-104">Here are two suggestions related to this:</span></span>

- <span data-ttu-id="b857e-105">Možete da pokušate da koristite [modul Exchange Online v2 PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps) koji uključuje CMDlet komande zasnovane na REST API-ju i koje imaju znatno bolje performanse.</span><span class="sxs-lookup"><span data-stu-id="b857e-105">You might want to try using the [Exchange Online v2 PowerShell module](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps), which includes CMDlets that are based on REST API and are significantly more performant.</span></span> <span data-ttu-id="b857e-106">Ovo može biti odlično rešenje za Get- CMDlet komande koje se često koriste.</span><span class="sxs-lookup"><span data-stu-id="b857e-106">This might be a great solution for a lot of Get- CMDlets that are frequently used.</span></span>
- <span data-ttu-id="b857e-107">Ako morate da koristite CMDlet komande koje još uvek nisu obuhvaćene v2 modulom, pogledajte članak [„Pokretanje PowerShell cmdlet komande za veliki broj korisnika u sistemu Office 365“](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#) koji govori o tome kako da zaobiđete očekivana PowerShell ograničenja u usluzi Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="b857e-107">If you need to use CMDlets that are not covered in the v2 module yet, please see [Running PowerShell cmdlets for large numbers of users in Office 365](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#), which talks about how to get around expected PowerShell throttling limits in Exchange Online.</span></span>
