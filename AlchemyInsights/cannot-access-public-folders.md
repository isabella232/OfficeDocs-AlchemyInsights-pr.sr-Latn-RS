---
title: Nije moguće pristupiti javnim fasciklama
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
- "3500007"
- "3462"
ms.openlocfilehash: af5bd57512ee917d6e22d3838d55a2a1d62750d4
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819526"
---
# <a name="outlook-cannot-connect-to-public-folders"></a><span data-ttu-id="892cf-102">Outlook ne može da se poveže sa javnim fasciklama</span><span class="sxs-lookup"><span data-stu-id="892cf-102">Outlook cannot connect to public folders</span></span>

<span data-ttu-id="892cf-103">Ako pristup javnoj fascikli ne funkcioniše za neke korisnike, pokušajte sledeće:</span><span class="sxs-lookup"><span data-stu-id="892cf-103">If public folder access isn't working for some users, try the following:</span></span>

<span data-ttu-id="892cf-104">Povežite se sa EXO PowerShell i konfigurišite DefaultPublicFolderMailbox parametar na problemnom korisničkom nalogu da bi se podudarao sa parametarom na radnom korisničkom nalogu.</span><span class="sxs-lookup"><span data-stu-id="892cf-104">Connect to EXO PowerShell and configure the DefaultPublicFolderMailbox parameter on the problem user account to match the parameter on a working user account.</span></span>

<span data-ttu-id="892cf-105">Primer:</span><span class="sxs-lookup"><span data-stu-id="892cf-105">Example:</span></span>

<span data-ttu-id="892cf-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span><span class="sxs-lookup"><span data-stu-id="892cf-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span></span>

<span data-ttu-id="892cf-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span><span class="sxs-lookup"><span data-stu-id="892cf-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span></span>

<span data-ttu-id="892cf-108">Sačekajte najmanje jedan čas da bi promena stupila na snagu.</span><span class="sxs-lookup"><span data-stu-id="892cf-108">Wait at least one hour for the change to take effect.</span></span>

<span data-ttu-id="892cf-109">Ako problem ostane, pratite ovu proceduru da biste rešili [probleme](https://aka.ms/pfcte) sa pristupom javnoj fascikli pomoću programa Outlook.</span><span class="sxs-lookup"><span data-stu-id="892cf-109">If the issue remains, please follow [this procedure](https://aka.ms/pfcte) to troubleshoot public folder access issues using Outlook.</span></span>
 
<span data-ttu-id="892cf-110">**Da biste kontrolisali koji korisnici mogu da pristupe javnim fasciklama pomoću programa Outlook:**</span><span class="sxs-lookup"><span data-stu-id="892cf-110">**To control which users can access public folders using Outlook**:</span></span>

1.  <span data-ttu-id="892cf-111">Koristite Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true ili $false</span><span class="sxs-lookup"><span data-stu-id="892cf-111">Use Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false</span></span>  
      
    <span data-ttu-id="892cf-112">$true: Dozvoljavanje korisnicima da pristupe javnim fasciklama u programu Outlook</span><span class="sxs-lookup"><span data-stu-id="892cf-112">$true: Allow users access public folders in Outlook</span></span>  
      
    <span data-ttu-id="892cf-113">$false: Sprečite korisnički pristup javnim fasciklama u programu Outlook.</span><span class="sxs-lookup"><span data-stu-id="892cf-113">$false: Prevent user access to public folders in Outlook.</span></span> <span data-ttu-id="892cf-114">Ovo je podrazumevana vrednost.</span><span class="sxs-lookup"><span data-stu-id="892cf-114">This is the default value.</span></span>  
        
2.  <span data-ttu-id="892cf-115">Set-OrganizationConfig -PublicFolderShowClientControl $true</span><span class="sxs-lookup"><span data-stu-id="892cf-115">Set-OrganizationConfig -PublicFolderShowClientControl $true</span></span>   
      
<span data-ttu-id="892cf-116">**Napomišite** Ova procedura može da kontroliše veze samo sa Outlook klijentima za računare za Windows.</span><span class="sxs-lookup"><span data-stu-id="892cf-116">**Note** This procedure can control connections only with Outlook desktop for Windows clients.</span></span> <span data-ttu-id="892cf-117">Korisnik može da nastavi da pristupa javnim fasciklama koristeći program OWA ili Outlook za Mac.</span><span class="sxs-lookup"><span data-stu-id="892cf-117">A user can continue accessing public folders using OWA or Outlook for Mac.</span></span>
 
<span data-ttu-id="892cf-118">Više informacija potražite u [članku Najavljivanje podrške za kontrolisane veze sa javnim fasciklama u programu Outlook.](https://aka.ms/controlpf)</span><span class="sxs-lookup"><span data-stu-id="892cf-118">For more info, see [Announcing Support for Controlled Connections to Public Folders in Outlook](https://aka.ms/controlpf).</span></span>