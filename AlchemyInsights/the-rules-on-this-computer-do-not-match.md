---
title: 'Greška: pravila na ovom kompjuteru se ne podudaraju'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "3518"
- "1800021"
ms.openlocfilehash: c0982da82826d1644f437b19e0d343a59d7ac473
ms.sourcegitcommit: e09af4285c6b81ca0a5320fdb811713ac25748c3
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 06/09/2020
ms.locfileid: "44664260"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a><span data-ttu-id="c4444-102">Greška: pravila na ovom kompjuteru se ne podudaraju</span><span class="sxs-lookup"><span data-stu-id="c4444-102">Error: The rules on this computer do not match</span></span>

<span data-ttu-id="c4444-103">Da biste videli ažurirani status ovog poznatog problema, pogledajte [pravila na ovom računaru ne podudaraju se sa pravilima na Microsoft Exchange serveru](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span><span class="sxs-lookup"><span data-stu-id="c4444-103">To see updated status of this known issue, see [The rules on this computer do not match the rules on Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span></span>

<span data-ttu-id="c4444-104">Outlook tim je implementirao ispravku u izradi 12928,10000.</span><span class="sxs-lookup"><span data-stu-id="c4444-104">The Outlook Team has implemented a fix in Build 12928.10000.</span></span> <span data-ttu-id="c4444-105">Popravka je već na izdanju Insider i ide na mesečni kanal krajem juna 2020.</span><span class="sxs-lookup"><span data-stu-id="c4444-105">The fix is already at Insider Fast and will go to Monthly Channel in late June 2020.</span></span> <span data-ttu-id="c4444-106">Kada budete imali fiksnu gradnju, možete dobiti Odzivnik "koja pravila želite da zadržite" poslednji put.</span><span class="sxs-lookup"><span data-stu-id="c4444-106">Once you have the fixed build you may get the prompt "Which rules do you want to keep" one last time.</span></span> <span data-ttu-id="c4444-107">Odaberite server kada se to od vas zatraži, a zatim se vratite u Outlook i ponovo omogućite sva pravila koja su onemogućena.</span><span class="sxs-lookup"><span data-stu-id="c4444-107">Choose Server when prompted and then go back in Outlook and re-enable any rules that were disabled.</span></span>

<span data-ttu-id="c4444-108">Dok ispravka ne bude dostupna, koristite sledeće rešenje:</span><span class="sxs-lookup"><span data-stu-id="c4444-108">Until the fix is available please use the following workaround:</span></span>

<span data-ttu-id="c4444-109">**Rešenje**: u poslednjim izveštajima došlo je do problema za one koji su kreirali samo pravila klijenta na radnoj površini programa Outlook.</span><span class="sxs-lookup"><span data-stu-id="c4444-109">**Workaround**: In recent reports, the issue has occurred for those that have only created client rules in Outlook desktop.</span></span> <span data-ttu-id="c4444-110">Ako i dalje budete u problemu, razmislite o brisanju pravila, a zatim kreirate i uređujete pravila samo u OWI (Outlook Web App) dok se problem ne razreši.</span><span class="sxs-lookup"><span data-stu-id="c4444-110">If you continue to run into the problem, consider deleting the rules and then create and edit rules only in OWA (Outlook Web App) until the issue is resolved.</span></span>

<span data-ttu-id="c4444-111">Ako ne možete ručno da izbrišete pravila, možete da pokrenete Outlook komandu kada pokrenete Outlook pokretanjem programa Outlook. exe/čistoza.</span><span class="sxs-lookup"><span data-stu-id="c4444-111">If you cannot delete the rules manually you can run an Outlook command when you start Outlook by running Outlook.exe /cleanrules.</span></span> <span data-ttu-id="c4444-112">Ovo će izbrisati i pravila klijenta i servera.</span><span class="sxs-lookup"><span data-stu-id="c4444-112">This will delete both the client and server rules.</span></span> <span data-ttu-id="c4444-113">Ona će izbrisati sva pravila za sve naloge u profilu programa Outlook.</span><span class="sxs-lookup"><span data-stu-id="c4444-113">It will delete all of the rules for all of the accounts in the Outlook Profile.</span></span> <span data-ttu-id="c4444-114">Ova komanda je detaljnije dokumentovana u članku sa parametrima komandne linije.</span><span class="sxs-lookup"><span data-stu-id="c4444-114">This command is further documented in the Command-line switches article.</span></span>

