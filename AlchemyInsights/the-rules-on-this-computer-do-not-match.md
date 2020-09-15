---
title: 'Greška: pravila na ovom računaru se ne podudaraju'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "3518"
- "1800021"
ms.openlocfilehash: c2feb6da651d8b3eb7af6a057335b28d26f9e7f6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47690977"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a><span data-ttu-id="2c391-102">Greška: pravila na ovom računaru se ne podudaraju</span><span class="sxs-lookup"><span data-stu-id="2c391-102">Error: The rules on this computer do not match</span></span>

<span data-ttu-id="2c391-103">Da biste videli ažurirani status ovog poznatog problema, pogledajte [pravila na ovom računaru se ne podudaraju sa pravilima u programu Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span><span class="sxs-lookup"><span data-stu-id="2c391-103">To see updated status of this known issue, see [The rules on this computer do not match the rules on Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span></span>

<span data-ttu-id="2c391-104">Outlook Team je sproveo ispravku u izdanju 12928,10000.</span><span class="sxs-lookup"><span data-stu-id="2c391-104">The Outlook Team has implemented a fix in Build 12928.10000.</span></span> <span data-ttu-id="2c391-105">Fiks je već u Unutraљnjoj brzoj usluzi Insider Fast i otići će na mesečni kanal krajem juna 2020.</span><span class="sxs-lookup"><span data-stu-id="2c391-105">The fix is already at Insider Fast and will go to Monthly Channel in late June 2020.</span></span> <span data-ttu-id="2c391-106">Kada imate fiksnu verziju, možda ćete dobiti odziv "koje pravilo želite da zadržite" poslednji put.</span><span class="sxs-lookup"><span data-stu-id="2c391-106">Once you have the fixed build you may get the prompt "Which rules do you want to keep" one last time.</span></span> <span data-ttu-id="2c391-107">Odaberite stavku server kada vam bude zatraženo, a zatim se vratite u Outlook i ponovo omogućite sva pravila koja su onemogućiti.</span><span class="sxs-lookup"><span data-stu-id="2c391-107">Choose Server when prompted and then go back in Outlook and re-enable any rules that were disabled.</span></span>

<span data-ttu-id="2c391-108">Dok ispravka ne bude dostupna koristite sledeće rešenje:</span><span class="sxs-lookup"><span data-stu-id="2c391-108">Until the fix is available please use the following workaround:</span></span>

<span data-ttu-id="2c391-109">**Zaobilaženje**problema: došlo je do problema za one koji imaju samo pravila klijenta u programu Outlook.</span><span class="sxs-lookup"><span data-stu-id="2c391-109">**Workaround**: In recent reports, the issue has occurred for those that have only created client rules in Outlook desktop.</span></span> <span data-ttu-id="2c391-110">Ako i dalje naiđete na problem, razmotrite Brisanje pravila, a zatim kreiranje i uređivanje pravila samo u programu OWA (Outlook Web App) dok se ne reši problem.</span><span class="sxs-lookup"><span data-stu-id="2c391-110">If you continue to run into the problem, consider deleting the rules and then create and edit rules only in OWA (Outlook Web App) until the issue is resolved.</span></span>

<span data-ttu-id="2c391-111">Ako pravila ne možete ručno da izbrišete, možete da pokrenete Outlook komandu kada pokrenete Outlook tako što ćete pokrenuti Outlook.exe/najиist.</span><span class="sxs-lookup"><span data-stu-id="2c391-111">If you cannot delete the rules manually you can run an Outlook command when you start Outlook by running Outlook.exe /cleanrules.</span></span> <span data-ttu-id="2c391-112">Ovo će izbrisati pravila klijenta i servera.</span><span class="sxs-lookup"><span data-stu-id="2c391-112">This will delete both the client and server rules.</span></span> <span data-ttu-id="2c391-113">Ona će izbrisati sva pravila za sve naloge u Outlook profilu.</span><span class="sxs-lookup"><span data-stu-id="2c391-113">It will delete all of the rules for all of the accounts in the Outlook Profile.</span></span> <span data-ttu-id="2c391-114">Ova komanda je dalje dokumentovana u članku Parametri komandne linije.</span><span class="sxs-lookup"><span data-stu-id="2c391-114">This command is further documented in the Command-line switches article.</span></span>

