---
title: 618 smernice za deljenje kalendara
ms.author: chrisda
author: chrisda
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "618"
- "899"
- "3800014"
ms.assetid: bc3db17b-87f8-4e50-b3ee-8b105b70d67a
ms.openlocfilehash: d2511183d068330cdcfb4e08b08df4f18625c822
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47684244"
---
# <a name="policy-error-when-sharing-a-calendar"></a><span data-ttu-id="418da-102">Greška u smernicama prilikom deljenja kalendara</span><span class="sxs-lookup"><span data-stu-id="418da-102">Policy error when sharing a calendar</span></span>

1. <span data-ttu-id="418da-103">Uradite nešto od sledećeg, u skladu sa situacijom:</span><span class="sxs-lookup"><span data-stu-id="418da-103">Do one of the following, as appropriate for your situation:</span></span>
    - <span data-ttu-id="418da-104">Povežite se sa uslugom Exchange online pomoću udaljenog PowerShell.</span><span class="sxs-lookup"><span data-stu-id="418da-104">Connect to Exchange Online by using Remote PowerShell.</span></span> <span data-ttu-id="418da-105">Više informacija potražite u članku [Povezivanje sa uslugom Exchange online pomoću udaljenog PowerShell](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="418da-105">For more information, see [Connect to Exchange Online using Remote PowerShell](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).</span></span>
    - <span data-ttu-id="418da-106">Na lokalnom serveru otvorite karticu upravljanje Exchange serverom.</span><span class="sxs-lookup"><span data-stu-id="418da-106">On the on-premises server, open the Exchange Management Shell.</span></span>
2. <span data-ttu-id="418da-107">Odredite smernice za deljenje koje su dodeljene korisniku.</span><span class="sxs-lookup"><span data-stu-id="418da-107">Determine the sharing policy that's assigned to the user.</span></span> <span data-ttu-id="418da-108">Da biste to uradili, izvršite sledeću komandu i napomena vraćene smernice:</span><span class="sxs-lookup"><span data-stu-id="418da-108">To do this, run the following command and note the policy returned:</span></span>

    `
    Get-Mailbox User1 | fl *sharing*
    `

3. <span data-ttu-id="418da-109">Ažurirajte smernice za deljenje za korisnika.</span><span class="sxs-lookup"><span data-stu-id="418da-109">Update the sharing policy for the user.</span></span> <span data-ttu-id="418da-110">Da biste to uradili, pratite ove korake:</span><span class="sxs-lookup"><span data-stu-id="418da-110">To do this, follow these steps:</span></span>
    - <span data-ttu-id="418da-111">Otvorite Exchange centar administracije.</span><span class="sxs-lookup"><span data-stu-id="418da-111">Open the Exchange admin center.</span></span>
    - <span data-ttu-id="418da-112">Izaberite stavku **organizacija**, a zatim kliknite dvaput na smernice koje su dodeljene korisniku u okviru **pojedinačno deljenje**.</span><span class="sxs-lookup"><span data-stu-id="418da-112">Click **Organization**, and then double-click the policy that's assigned to the user under **Individual Sharing**.</span></span> <span data-ttu-id="418da-113">Ovo su smernice vraćene u 2.</span><span class="sxs-lookup"><span data-stu-id="418da-113">This is the policy that was returned in step 2.</span></span>
    - <span data-ttu-id="418da-114">Na stranici pravilo za deljenje izaberite nivo deljenja kalendara koji želite da omogućite u okviru **navedite koje informacije želite da delite**; Kliknite na dugme **Sačuvaj**.</span><span class="sxs-lookup"><span data-stu-id="418da-114">On the Sharing Rule page, select the calendar sharing level that you want to allow under **Specify what information you want to share**; click **Save**.</span></span>

<span data-ttu-id="418da-115">Više informacija potražite u članku: ["smernice ne dozvole dodeljivanje dozvola na ovom nivou jednoj ili više primalaca" kada korisnik pokuša da deli kalendar](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue).</span><span class="sxs-lookup"><span data-stu-id="418da-115">For more information see: ["Policy does not allow granting permissions at this level to one or more of the recipient(s)" error when user tries to share calendar](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue).</span></span>
