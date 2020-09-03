---
title: Nije moguće pristupiti javnim fasciklama
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: d63a193585cb73c2ce8e160d413db4e837100d33
ms.sourcegitcommit: d3ace2376195d54229ee1e232daf8133ba4e58a9
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/03/2020
ms.locfileid: "47341417"
---
# <a name="outlook-cannot-connect-to-public-folders"></a><span data-ttu-id="22c0a-102">Outlook ne može da se poveže sa javnim fasciklama</span><span class="sxs-lookup"><span data-stu-id="22c0a-102">Outlook cannot connect to public folders</span></span>

<span data-ttu-id="22c0a-103">Ako pristup javnoj fascikli ne radi za neke korisnike, Isprobajte sledeće:</span><span class="sxs-lookup"><span data-stu-id="22c0a-103">If public folder access isn't working for some users, try the following:</span></span>

<span data-ttu-id="22c0a-104">Povežite se sa EXO PowerShell i konfigurišite parametar Defaultpublicfolfoldersanduče na problem korisničkog naloga da bi se podudarao sa parametrima na radnom korisničkom nalogu.</span><span class="sxs-lookup"><span data-stu-id="22c0a-104">Connect to EXO PowerShell and configure the DefaultPublicFolderMailbox parameter on the problem user account to match the parameter on a working user account.</span></span>

<span data-ttu-id="22c0a-105">Primer</span><span class="sxs-lookup"><span data-stu-id="22c0a-105">Example:</span></span>

<span data-ttu-id="22c0a-106">Rešenje "Uzmi-poštansko sanduče" | FT Defaultpublicfolfolderpoštansko sanduče, efikasno iskorišćenost poštanskog sandučeta</span><span class="sxs-lookup"><span data-stu-id="22c0a-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span></span>

<span data-ttu-id="22c0a-107">Komplet-problem sa poštanskim sandučetom-Defaultpublicfoldersanduče \<value from previous command></span><span class="sxs-lookup"><span data-stu-id="22c0a-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span></span>

<span data-ttu-id="22c0a-108">Sačekajte najmanje jedan sat da bi promena stupila na snagu.</span><span class="sxs-lookup"><span data-stu-id="22c0a-108">Wait at least one hour for the change to take effect.</span></span>

<span data-ttu-id="22c0a-109">Ako problem ostane, pratite [ovu proceduru](https://aka.ms/pfcte) da biste rešili probleme sa pristupom javnoj fascikli pomoću programa Outlook.</span><span class="sxs-lookup"><span data-stu-id="22c0a-109">If the issue remains, please follow [this procedure](https://aka.ms/pfcte) to troubleshoot public folder access issues using Outlook.</span></span>
 
<span data-ttu-id="22c0a-110">**Da biste kontrolisali koji korisnici mogu da pristupe javnim fasciklama pomoću programa Outlook**:</span><span class="sxs-lookup"><span data-stu-id="22c0a-110">**To control which users can access public folders using Outlook**:</span></span>

1.  <span data-ttu-id="22c0a-111">Koristite setu- <mailboxname> Kaskadepoštansko sanduče-publicfolderclientaccess $TRUE ili $FALSE</span><span class="sxs-lookup"><span data-stu-id="22c0a-111">Use Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false</span></span>  
      
    <span data-ttu-id="22c0a-112">$true: Omogućavanje korisnicima da pristupaju javnim fasciklama u programu Outlook</span><span class="sxs-lookup"><span data-stu-id="22c0a-112">$true: Allow users access public folders in Outlook</span></span>  
      
    <span data-ttu-id="22c0a-113">$false: sprečite korisnički pristup javnim fasciklama u programu Outlook.</span><span class="sxs-lookup"><span data-stu-id="22c0a-113">$false: Prevent user access to public folders in Outlook.</span></span> <span data-ttu-id="22c0a-114">Ovo je podrazumevana vrednost.</span><span class="sxs-lookup"><span data-stu-id="22c0a-114">This is the default value.</span></span>  
        
2.  <span data-ttu-id="22c0a-115">Scenokonfiguracija – Publicfoldershow$TRUE</span><span class="sxs-lookup"><span data-stu-id="22c0a-115">Set-OrganizationConfig -PublicFolderShowClientControl $true</span></span>   
      
<span data-ttu-id="22c0a-116">**Napomena** Ova procedura može da kontroliše veze samo sa Outlook klijentima za računare za Windows.</span><span class="sxs-lookup"><span data-stu-id="22c0a-116">**Note** This procedure can control connections only with Outlook desktop for Windows clients.</span></span> <span data-ttu-id="22c0a-117">Korisnik može da nastavi pristup javnim fasciklama pomoću aplikacije OWA ili Outlook za Mac.</span><span class="sxs-lookup"><span data-stu-id="22c0a-117">A user can continue accessing public folders using OWA or Outlook for Mac.</span></span>
 
<span data-ttu-id="22c0a-118">Više informacija potražite u članku [Najavljujemo podršku za kontrolisane veze ka javnim fasciklama u programu Outlook](https://aka.ms/controlpf).</span><span class="sxs-lookup"><span data-stu-id="22c0a-118">For more info, see [Announcing Support for Controlled Connections to Public Folders in Outlook](https://aka.ms/controlpf).</span></span>