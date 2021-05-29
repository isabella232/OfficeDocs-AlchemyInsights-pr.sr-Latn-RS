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
ms.openlocfilehash: 204e0248bc2f07f14fa789d1d2999495910ee034
ms.sourcegitcommit: d2108b13acc44e26b65f9a2739cbce9bf98959a5
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 05/28/2021
ms.locfileid: "52702140"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a><span data-ttu-id="bbab6-102">Mikro kašnjenja ili ograničavanje u usluzi Exchange Online PowerShell</span><span class="sxs-lookup"><span data-stu-id="bbab6-102">Micro delays or throttling in Exchange Online PowerShell</span></span>

<span data-ttu-id="bbab6-103">Možda ćete videti upozorenja „Primenjeno je mikro kašnjenje“ ili kašnjenja kada pokrenete skripte ili cmdlet komande u usluzi Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="bbab6-103">You might see "Micro delay applied" warnings or delays when you run scripts and cmdlets in Exchange Online.</span></span> <span data-ttu-id="bbab6-104">Evo nekoliko predloga kako da rešite ovo:</span><span class="sxs-lookup"><span data-stu-id="bbab6-104">Here are a few suggestions how to solve this:</span></span>

- <span data-ttu-id="bbab6-105">Pokrenite našu dijagnostiku da biste opustili PowerShell smernice za zakupca.</span><span class="sxs-lookup"><span data-stu-id="bbab6-105">Please run our diagnostics to relax your tenant's PowerShell throttling policies.</span></span> <span data-ttu-id="bbab6-106">Ovo rešenje će rešiti problem za većinu.</span><span class="sxs-lookup"><span data-stu-id="bbab6-106">This solution will solve the problem for most.</span></span>
- <span data-ttu-id="bbab6-107">Ako problem još uvek nije rešen, [koristite Exchange Online v2 PowerShell modul,](/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps&preserve-view=true)koji obuhvata CMDlet komande koje su zasnovane na REST API-u i znatno su performantnije.</span><span class="sxs-lookup"><span data-stu-id="bbab6-107">If issue still not solved, use the [Exchange Online v2 PowerShell module](/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps&preserve-view=true), which includes CMDlets that are based on REST API and are significantly more performant.</span></span> <span data-ttu-id="bbab6-108">Ovo može biti odlično rešenje za Get- CMDlet komande koje se često koriste.</span><span class="sxs-lookup"><span data-stu-id="bbab6-108">This might be a great solution for a lot of Get- CMDlets that are frequently used.</span></span>
- <span data-ttu-id="bbab6-109">Ako treba da koristite CMDlet komande koje nisu pokrivene v2 modulom, pročitajte tj. Pokretanje [PowerShell cmdlet](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#)komandi za veliki broj korisnika u programu Office 365 , što govori o tome kako da zaobičete PowerShell ograničenja za ograničavanje u Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="bbab6-109">If you need to use CMDlets that are not covered in the v2 module, please see [Running PowerShell cmdlets for large numbers of users in Office 365](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#), which talks about how to get around PowerShell throttling limits in Exchange Online.</span></span>
