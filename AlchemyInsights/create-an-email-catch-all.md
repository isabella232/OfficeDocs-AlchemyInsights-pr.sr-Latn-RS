---
title: Kreiranje e-poruke
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
- "9001524"
- "3732"
ms.openlocfilehash: 262d2c6a7181d94094f3d840c4ba3ebd07000cf4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47713000"
---
# <a name="create-an-email-catch-all"></a><span data-ttu-id="950aa-102">Kreiranje e-poruke</span><span class="sxs-lookup"><span data-stu-id="950aa-102">Create an email catch all</span></span>

<span data-ttu-id="950aa-103">Upotreba hvatanja je odlučno obeshrabrena.</span><span class="sxs-lookup"><span data-stu-id="950aa-103">Use of a catch all is strongly discouraged.</span></span> <span data-ttu-id="950aa-104">Bolje je da se ponovo vratite na pošiljalac koji omogućava pošiljaoce da saznaju da poruka nije mogla da se dostavi kao adresirana kako bi mogla da preduzme radnju.</span><span class="sxs-lookup"><span data-stu-id="950aa-104">It is better to provide a bounce back to the sender letting senders know their message could not be delivered as addressed so they can take action.</span></span> <span data-ttu-id="950aa-105">Praćenom poštanskom sandučetu možete da ograničite samo da biste imali važeće e-adrese.</span><span class="sxs-lookup"><span data-stu-id="950aa-105">You can also limit the monitored mailbox to only catch formerly valid email addresses.</span></span> 

<span data-ttu-id="950aa-106">Bilo koji ulov sve poštansko sanduče dobiće dobar deo bezvredne pošte i može na kraju popuniti ako se pažljivo ne nadgleda.</span><span class="sxs-lookup"><span data-stu-id="950aa-106">Any catch all mailbox will receive a good deal of spam and may eventually fill if not closely monitored.</span></span> <span data-ttu-id="950aa-107">(Postoje ograničenja za primanje.)</span><span class="sxs-lookup"><span data-stu-id="950aa-107">(There are receiving limits.)</span></span> 

<span data-ttu-id="950aa-108">Ako odlučite da nastavite, pratite ove korake:</span><span class="sxs-lookup"><span data-stu-id="950aa-108">If you decide to proceed, follow these steps:</span></span>

1. <span data-ttu-id="950aa-109">Kreirajte dinamičku grupu za distribuciju & uključujete "sve tipove primalaca".</span><span class="sxs-lookup"><span data-stu-id="950aa-109">Create a Dynamic Distribution Group & include "All Recipient Types."</span></span>

2. <span data-ttu-id="950aa-110">Kreiranje namenskog poštanskog sandučeta za hvatanje e-poruka, na primer, catchall@domain.com.</span><span class="sxs-lookup"><span data-stu-id="950aa-110">Create a dedicated Mailbox to catch emails, for example, catchall@domain.com.</span></span>

3. <span data-ttu-id="950aa-111">Za određeni domen, postavljanje domena za domen "Inter".</span><span class="sxs-lookup"><span data-stu-id="950aa-111">For the specific domain, set the DomainType to “InternalRelay”.</span></span> <span data-ttu-id="950aa-112">Ako kasnije uklonite sve hvatanje, obavezno ponovo konfigurišete domen za autoritativno.</span><span class="sxs-lookup"><span data-stu-id="950aa-112">If you later remove the catch all, be sure to set the domain back to Authoritative.</span></span>

4. <span data-ttu-id="950aa-113">Kreirajte pravilo transporta Pošilka na sledeći način:</span><span class="sxs-lookup"><span data-stu-id="950aa-113">Create a Mailflow Transport Rule as follows:</span></span>

    - <span data-ttu-id="950aa-114">Ako je pošiljalac "izvan organizacije"</span><span class="sxs-lookup"><span data-stu-id="950aa-114">If the Sender is "Outside the Organization"</span></span>
    - <span data-ttu-id="950aa-115">Preusmeravanje poruke na Catchall@domain.com</span><span class="sxs-lookup"><span data-stu-id="950aa-115">Redirect the message to Catchall@domain.com</span></span>
    - <span data-ttu-id="950aa-116">Osim ako je primalac član allusers@domain.com (grupna raspodela sadrži sve članove)</span><span class="sxs-lookup"><span data-stu-id="950aa-116">Except if the recipient is a member of allusers@domain.com (Distribution Group contains all members)</span></span>
    - <span data-ttu-id="950aa-117">Uverite se da su novi poštanski sandučići dodati u grupu za dinamiku distribucije</span><span class="sxs-lookup"><span data-stu-id="950aa-117">Ensure to validate that new mailboxes are added into the Dynamic Distribution Group</span></span>
