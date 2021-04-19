---
title: Kontrola pristupa javnim fasciklama pomoću programa Outlook
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
- "3500007"
- "3462"
ms.openlocfilehash: f528044ca7f6f2ee2812f9f831093c44eca26fe1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816754"
---
# <a name="control-access-to-public-folders-using-outlook"></a><span data-ttu-id="45eef-102">Kontrola pristupa javnim fasciklama pomoću programa Outlook</span><span class="sxs-lookup"><span data-stu-id="45eef-102">Control access to public folders using Outlook</span></span>

<span data-ttu-id="45eef-103">Da biste kontrolisali koji korisnici mogu da pristupe javnim fasciklama pomoću programa Outlook:</span><span class="sxs-lookup"><span data-stu-id="45eef-103">To control which users can access public folders using Outlook:</span></span>

1. <span data-ttu-id="45eef-104">Koristite `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`</span><span class="sxs-lookup"><span data-stu-id="45eef-104">Use `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`</span></span>

<span data-ttu-id="45eef-105">$true: Dozvoljavanje korisnicima da pristupe javnim fasciklama u programu Outlook</span><span class="sxs-lookup"><span data-stu-id="45eef-105">$true: Allow users access public folders in Outlook</span></span>  
<span data-ttu-id="45eef-106">$false: Sprečite korisnički pristup javnim fasciklama u programu Outlook.</span><span class="sxs-lookup"><span data-stu-id="45eef-106">$false: Prevent user access to public folders in Outlook.</span></span> <span data-ttu-id="45eef-107">Ovo je podrazumevana vrednost.</span><span class="sxs-lookup"><span data-stu-id="45eef-107">This is the default value.</span></span>  

2. `Set-OrganizationConfig -PublicFolderShowClientControl $true`

<span data-ttu-id="45eef-108">Napom: Ova procedura može da kontroliše samo veze sa Outlook klijentima za računare za Windows.</span><span class="sxs-lookup"><span data-stu-id="45eef-108">Note: This procedure can only control connections with Outlook desktop for Windows clients.</span></span> <span data-ttu-id="45eef-109">Korisnici mogu da nastave da pristupe javnim fasciklama koristeći program OWA ili Outlook za Mac.</span><span class="sxs-lookup"><span data-stu-id="45eef-109">Users can continue accessing public folders using OWA or Outlook for Mac.</span></span>

<span data-ttu-id="45eef-110">Dodatne informacije potražite u [temi Kontrolisane veze sa javnim fasciklama u programu Outlook](https://aka.ms/controlpf) za više informacija.</span><span class="sxs-lookup"><span data-stu-id="45eef-110">For more information, see [Controlled Connections to Public Folders in Outlook](https://aka.ms/controlpf) for more information.</span></span>
