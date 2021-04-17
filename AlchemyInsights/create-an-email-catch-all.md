---
title: Napravite e-poruku koja se hvata sve
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
- "9001524"
- "3732"
ms.openlocfilehash: 2b9131a620139a93ddb844fd49d8fa2ed68e52c2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816214"
---
# <a name="create-an-email-catch-all"></a><span data-ttu-id="a342d-102">Napravite e-poruku koja se hvata sve</span><span class="sxs-lookup"><span data-stu-id="a342d-102">Create an email catch all</span></span>

<span data-ttu-id="a342d-103">Upotreba zahladanja je veoma odsutan.</span><span class="sxs-lookup"><span data-stu-id="a342d-103">Use of a catch all is strongly discouraged.</span></span> <span data-ttu-id="a342d-104">Bolje je da obezbedite odskok pošiljaocu i tako ga pustite da zna da nije moguće isporučiti poruku kako bi mogli da preduzme radnju.</span><span class="sxs-lookup"><span data-stu-id="a342d-104">It is better to provide a bounce back to the sender letting senders know their message could not be delivered as addressed so they can take action.</span></span> <span data-ttu-id="a342d-105">Takođe možete da ograničite nadgledano poštansko sanduče tako da prima samo ranije važeće e-adrese.</span><span class="sxs-lookup"><span data-stu-id="a342d-105">You can also limit the monitored mailbox to only catch formerly valid email addresses.</span></span> 

<span data-ttu-id="a342d-106">Svako hvatanje svakog poštanskog sandučeta dobiće dobru ponudu bezb. I na kraju ih može popuniti ako se ne nadgleda pažljivo.</span><span class="sxs-lookup"><span data-stu-id="a342d-106">Any catch all mailbox will receive a good deal of spam and may eventually fill if not closely monitored.</span></span> <span data-ttu-id="a342d-107">(Postoje ograničenja za prijem.)</span><span class="sxs-lookup"><span data-stu-id="a342d-107">(There are receiving limits.)</span></span> 

<span data-ttu-id="a342d-108">Ako odlučite da nastavite, pratite ove korake:</span><span class="sxs-lookup"><span data-stu-id="a342d-108">If you decide to proceed, follow these steps:</span></span>

1. <span data-ttu-id="a342d-109">Kreiranje dinamičke grupe za distribuciju & "Svi tipovi primalaca".</span><span class="sxs-lookup"><span data-stu-id="a342d-109">Create a Dynamic Distribution Group & include "All Recipient Types."</span></span>

2. <span data-ttu-id="a342d-110">Kreirajte namenski poštansko sanduče da biste hvatali e-poruke, na primer catchall@domain.com.</span><span class="sxs-lookup"><span data-stu-id="a342d-110">Create a dedicated Mailbox to catch emails, for example, catchall@domain.com.</span></span>

3. <span data-ttu-id="a342d-111">Za određeni domen podesite DomainType na "InternalRelay".</span><span class="sxs-lookup"><span data-stu-id="a342d-111">For the specific domain, set the DomainType to “InternalRelay”.</span></span> <span data-ttu-id="a342d-112">Ako kasnije uklonite sve stavke, uverite se da ste domen vratili na "Ovlašćeno".</span><span class="sxs-lookup"><span data-stu-id="a342d-112">If you later remove the catch all, be sure to set the domain back to Authoritative.</span></span>

4. <span data-ttu-id="a342d-113">Kreirajte pravilo za prenos toka pošte na sledeći način:</span><span class="sxs-lookup"><span data-stu-id="a342d-113">Create a Mailflow Transport Rule as follows:</span></span>

    - <span data-ttu-id="a342d-114">Ako pošiljalac ima "Izvan organizacije"</span><span class="sxs-lookup"><span data-stu-id="a342d-114">If the Sender is "Outside the Organization"</span></span>
    - <span data-ttu-id="a342d-115">Preusmerite poruku na Catchall@domain.com</span><span class="sxs-lookup"><span data-stu-id="a342d-115">Redirect the message to Catchall@domain.com</span></span>
    - <span data-ttu-id="a342d-116">Osim ako je primalac član grupe allusers@domain.com (grupa za distribuciju sadrži sve članove)</span><span class="sxs-lookup"><span data-stu-id="a342d-116">Except if the recipient is a member of allusers@domain.com (Distribution Group contains all members)</span></span>
    - <span data-ttu-id="a342d-117">Proverite da li je provera valjanosti novih poštanskih sandučića dodata u dinamičkoj grupi za distribuciju</span><span class="sxs-lookup"><span data-stu-id="a342d-117">Ensure to validate that new mailboxes are added into the Dynamic Distribution Group</span></span>
