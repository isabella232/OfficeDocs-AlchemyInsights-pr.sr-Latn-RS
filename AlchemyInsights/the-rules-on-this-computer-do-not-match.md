---
title: 'Greška: Pravila na ovom računaru se ne podudaraju'
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "3518"
- "1800021"
ms.openlocfilehash: c46eb856baafbef9bc3b7fa34a0258ef16923fb8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/15/2021
ms.locfileid: "51782966"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a><span data-ttu-id="7e36c-102">Greška: Pravila na ovom računaru se ne podudaraju</span><span class="sxs-lookup"><span data-stu-id="7e36c-102">Error: The rules on this computer do not match</span></span>

<span data-ttu-id="7e36c-103">Da biste videli ažurirani status ovog poznatog problema, pogledajte članak Pravila na ovom računaru se ne podudaraju sa [pravilima u sistemu Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span><span class="sxs-lookup"><span data-stu-id="7e36c-103">To see updated status of this known issue, see [The rules on this computer do not match the rules on Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span></span>

<span data-ttu-id="7e36c-104">Outlook tim je primenio ispravku u verzija 12928.10000.</span><span class="sxs-lookup"><span data-stu-id="7e36c-104">The Outlook Team has implemented a fix in Build 12928.10000.</span></span> <span data-ttu-id="7e36c-105">Popravka je već u 2013. insajderu i biće prešla na mesečni kanal krajem juna 2020.</span><span class="sxs-lookup"><span data-stu-id="7e36c-105">The fix is already at Insider Fast and will go to Monthly Channel in late June 2020.</span></span> <span data-ttu-id="7e36c-106">Kada imate fiksno pravilo, poslednji put možete da dobijete odziv "Koja pravila želite da zadržite".</span><span class="sxs-lookup"><span data-stu-id="7e36c-106">Once you have the fixed build you may get the prompt "Which rules do you want to keep" one last time.</span></span> <span data-ttu-id="7e36c-107">Odaberite stavku Server kada vam to bude zatraženo, a zatim se vratite u program Outlook i ponovo omogućite pravila koja su onemogućena.</span><span class="sxs-lookup"><span data-stu-id="7e36c-107">Choose Server when prompted and then go back in Outlook and re-enable any rules that were disabled.</span></span>

<span data-ttu-id="7e36c-108">Dok ispravka ne bude dostupna, koristite sledeće rešenje:</span><span class="sxs-lookup"><span data-stu-id="7e36c-108">Until the fix is available please use the following workaround:</span></span>

<span data-ttu-id="7e36c-109">**Zaostalo je** problem: U nedavnim izveštajima došlo je do problema za one koji su kreirali pravila klijenta samo u programu Outlook za računare.</span><span class="sxs-lookup"><span data-stu-id="7e36c-109">**Workaround**: In recent reports, the issue has occurred for those that have only created client rules in Outlook desktop.</span></span> <span data-ttu-id="7e36c-110">Ako i dalje naiđete na problem, razmotrite brisanje pravila, a zatim pravite i uređujte pravila samo u programu OWA (Outlook Web App) dok se problem ne reši.</span><span class="sxs-lookup"><span data-stu-id="7e36c-110">If you continue to run into the problem, consider deleting the rules and then create and edit rules only in OWA (Outlook Web App) until the issue is resolved.</span></span>

<span data-ttu-id="7e36c-111">Ako pravila ne možete ručno da izbrišete, možete da pokrenete Outlook komandu kada pokrenete Outlook tako što ćete pokrenuti Outlook.exe /cleanrules.</span><span class="sxs-lookup"><span data-stu-id="7e36c-111">If you cannot delete the rules manually you can run an Outlook command when you start Outlook by running Outlook.exe /cleanrules.</span></span> <span data-ttu-id="7e36c-112">Ovo će izbrisati i pravila klijenta i servera.</span><span class="sxs-lookup"><span data-stu-id="7e36c-112">This will delete both the client and server rules.</span></span> <span data-ttu-id="7e36c-113">To će izbrisati sva pravila za sve naloge u Outlook profilu.</span><span class="sxs-lookup"><span data-stu-id="7e36c-113">It will delete all of the rules for all of the accounts in the Outlook Profile.</span></span> <span data-ttu-id="7e36c-114">Ova komanda je dodatno dokumentovana u članku Prekidači komandne linije.</span><span class="sxs-lookup"><span data-stu-id="7e36c-114">This command is further documented in the Command-line switches article.</span></span>

