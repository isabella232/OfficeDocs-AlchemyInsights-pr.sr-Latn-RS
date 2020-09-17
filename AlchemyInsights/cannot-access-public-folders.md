---
title: Nije moguće pristupiti javnim fasciklama
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
- "3500007"
- "3462"
ms.openlocfilehash: 272918b38f6019cb2bdcaa4013baebaa5f04fe85
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/15/2020
ms.locfileid: "47812561"
---
# <a name="outlook-cannot-connect-to-public-folders"></a><span data-ttu-id="be10f-102">Outlook ne može da se poveže sa javnim fasciklama</span><span class="sxs-lookup"><span data-stu-id="be10f-102">Outlook cannot connect to public folders</span></span>

<span data-ttu-id="be10f-103">Ako pristup javnoj fascikli ne radi za neke korisnike, Isprobajte sledeće:</span><span class="sxs-lookup"><span data-stu-id="be10f-103">If public folder access isn't working for some users, try the following:</span></span>

<span data-ttu-id="be10f-104">Povežite se sa EXO PowerShell i konfigurišite parametar Defaultpublicfolfoldersanduče na problem korisničkog naloga da bi se podudarao sa parametrima na radnom korisničkom nalogu.</span><span class="sxs-lookup"><span data-stu-id="be10f-104">Connect to EXO PowerShell and configure the DefaultPublicFolderMailbox parameter on the problem user account to match the parameter on a working user account.</span></span>

<span data-ttu-id="be10f-105">Primer</span><span class="sxs-lookup"><span data-stu-id="be10f-105">Example:</span></span>

<span data-ttu-id="be10f-106">Rešenje "Uzmi-poštansko sanduče" | FT Defaultpublicfolfolderpoštansko sanduče, efikasno iskorišćenost poštanskog sandučeta</span><span class="sxs-lookup"><span data-stu-id="be10f-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span></span>

<span data-ttu-id="be10f-107">Komplet-problem sa poštanskim sandučetom-Defaultpublicfoldersanduče \<value from previous command></span><span class="sxs-lookup"><span data-stu-id="be10f-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span></span>

<span data-ttu-id="be10f-108">Sačekajte najmanje jedan sat da bi promena stupila na snagu.</span><span class="sxs-lookup"><span data-stu-id="be10f-108">Wait at least one hour for the change to take effect.</span></span>

<span data-ttu-id="be10f-109">Ako problem ostane, pratite [ovu proceduru](https://aka.ms/pfcte) da biste rešili probleme sa pristupom javnoj fascikli pomoću programa Outlook.</span><span class="sxs-lookup"><span data-stu-id="be10f-109">If the issue remains, please follow [this procedure](https://aka.ms/pfcte) to troubleshoot public folder access issues using Outlook.</span></span>
 
<span data-ttu-id="be10f-110">**Da biste kontrolisali koji korisnici mogu da pristupe javnim fasciklama pomoću programa Outlook**:</span><span class="sxs-lookup"><span data-stu-id="be10f-110">**To control which users can access public folders using Outlook**:</span></span>

1.  <span data-ttu-id="be10f-111">Koristite setu- <mailboxname> Kaskadepoštansko sanduče-publicfolderclientaccess $TRUE ili $FALSE</span><span class="sxs-lookup"><span data-stu-id="be10f-111">Use Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false</span></span>  
      
    <span data-ttu-id="be10f-112">$true: Omogućavanje korisnicima da pristupaju javnim fasciklama u programu Outlook</span><span class="sxs-lookup"><span data-stu-id="be10f-112">$true: Allow users access public folders in Outlook</span></span>  
      
    <span data-ttu-id="be10f-113">$false: sprečite korisnički pristup javnim fasciklama u programu Outlook.</span><span class="sxs-lookup"><span data-stu-id="be10f-113">$false: Prevent user access to public folders in Outlook.</span></span> <span data-ttu-id="be10f-114">Ovo je podrazumevana vrednost.</span><span class="sxs-lookup"><span data-stu-id="be10f-114">This is the default value.</span></span>  
        
2.  <span data-ttu-id="be10f-115">Scenokonfiguracija – Publicfoldershow$TRUE</span><span class="sxs-lookup"><span data-stu-id="be10f-115">Set-OrganizationConfig -PublicFolderShowClientControl $true</span></span>   
      
<span data-ttu-id="be10f-116">**Napomena** Ova procedura može da kontroliše veze samo sa Outlook klijentima za računare za Windows.</span><span class="sxs-lookup"><span data-stu-id="be10f-116">**Note** This procedure can control connections only with Outlook desktop for Windows clients.</span></span> <span data-ttu-id="be10f-117">Korisnik može da nastavi pristup javnim fasciklama pomoću aplikacije OWA ili Outlook za Mac.</span><span class="sxs-lookup"><span data-stu-id="be10f-117">A user can continue accessing public folders using OWA or Outlook for Mac.</span></span>
 
<span data-ttu-id="be10f-118">Više informacija potražite u članku [Najavljujemo podršku za kontrolisane veze ka javnim fasciklama u programu Outlook](https://aka.ms/controlpf).</span><span class="sxs-lookup"><span data-stu-id="be10f-118">For more info, see [Announcing Support for Controlled Connections to Public Folders in Outlook](https://aka.ms/controlpf).</span></span>