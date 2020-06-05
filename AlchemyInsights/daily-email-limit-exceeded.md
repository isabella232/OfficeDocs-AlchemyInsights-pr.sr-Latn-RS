---
title: Premašen je dnevni limit e-pošte. Tok posla je obustavljen.
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: 701c4aef6bfc0c4a2c4570f6dd16dbe4f99efc44
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580347"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a><span data-ttu-id="c49d8-103">Premašen je dnevni limit e-pošte.</span><span class="sxs-lookup"><span data-stu-id="c49d8-103">Daily email Limit Exceeded.</span></span> <span data-ttu-id="c49d8-104">Tok posla je obustavljen.</span><span class="sxs-lookup"><span data-stu-id="c49d8-104">Workflow is suspended.</span></span>

<span data-ttu-id="c49d8-105">Ova greška može biti primljena u sledećim slučajevima:</span><span class="sxs-lookup"><span data-stu-id="c49d8-105">This error may be received in the following scenarios:</span></span>

- <span data-ttu-id="c49d8-106">Imate tok posla na SharePoint mreži koji koristi tip platforme SharePoint 2010 ili SharePoint 2013 Workflow.</span><span class="sxs-lookup"><span data-stu-id="c49d8-106">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>
- <span data-ttu-id="c49d8-107">Tok posla je konfigurisan da šalje prilagođenu e-poruku u više od 200 korisnika u isto vreme, više od 10.000 primalaca dnevno ili više od 30 poruka u minuti.</span><span class="sxs-lookup"><span data-stu-id="c49d8-107">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>
- <span data-ttu-id="c49d8-108">Kada pokrenete tok posla, e-poruka se ne šalje i primetićete sledeće ponašanje:</span><span class="sxs-lookup"><span data-stu-id="c49d8-108">When you run the workflow, the email message isn't sent, and you notice the following behavior:</span></span>
    - <span data-ttu-id="c49d8-109">Za tok posla koji koristi tip SharePoint 2013 platforme, potražite stranicu " **Status toka posla** ".</span><span class="sxs-lookup"><span data-stu-id="c49d8-109">For a workflow using the SharePoint 2013 platform type, you browse to the **Workflow Status** page.</span></span> <span data-ttu-id="c49d8-110">Na stranici "Status toka posla", **unutrašnji status** je postavljen na " **pokrenuto**", a "informacioni balon" **ne može da pošalje primaocu**.</span><span class="sxs-lookup"><span data-stu-id="c49d8-110">On the Workflow Status page, the **Internal Status** is set to **Started**, and the information balloon displays **Unable to send to a recipient**.</span></span>

<span data-ttu-id="c49d8-111">Da biste zaobišli ovaj problem, konfigurišite tok posla za slanje e-poruka bez prekoračenja [ograničenja za Exchange online](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span><span class="sxs-lookup"><span data-stu-id="c49d8-111">To work around this issue, configure your workflow to send email messages without exceeding the [Exchange Online sender limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span></span> <span data-ttu-id="c49d8-112">Na primer, koristite pauzu u toku posla, pošaljite e-poruku u Microsoft 365 grupu, grupu za distribuciju ili bezbednosnu grupu za koju je omogućena pošta ili pošaljite poruku na manje od 200 primalaca.</span><span class="sxs-lookup"><span data-stu-id="c49d8-112">For example, use a pause in the workflow, send the email to a Microsoft 365 group, a distribution group or mail enabled security group, or send the message to fewer than 200 recipients at a time.</span></span>


<span data-ttu-id="c49d8-113">Više informacija potražite u sledećem [članku](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).</span><span class="sxs-lookup"><span data-stu-id="c49d8-113">For more information, see the following [article](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).</span></span>

## <a name="related-topics"></a><span data-ttu-id="c49d8-114">Povezane teme</span><span class="sxs-lookup"><span data-stu-id="c49d8-114">Related topics</span></span>
- [<span data-ttu-id="c49d8-115">Kreiraj tok</span><span class="sxs-lookup"><span data-stu-id="c49d8-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="c49d8-116">SharePoint i protok</span><span class="sxs-lookup"><span data-stu-id="c49d8-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 