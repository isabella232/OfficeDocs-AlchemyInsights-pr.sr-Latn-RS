---
title: Dnevno ograničenje za svakodnevne e-poštu. Tok posla obustavljen.
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: dfb42b24f1c2b4b05cb067a82505a6a8b63f277e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47731577"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a><span data-ttu-id="d3bfd-103">Dnevno ograničenje za svakodnevne e-poštu.</span><span class="sxs-lookup"><span data-stu-id="d3bfd-103">Daily email Limit Exceeded.</span></span> <span data-ttu-id="d3bfd-104">Tok posla obustavljen.</span><span class="sxs-lookup"><span data-stu-id="d3bfd-104">Workflow is suspended.</span></span>

<span data-ttu-id="d3bfd-105">Ova greška se može primiti u sledećim slučajevima:</span><span class="sxs-lookup"><span data-stu-id="d3bfd-105">This error may be received in the following scenarios:</span></span>

- <span data-ttu-id="d3bfd-106">Imate tok posla u sistemu SharePoint online koji koristi SharePoint 2010 ili SharePoint 2013 tip platforme toka posla.</span><span class="sxs-lookup"><span data-stu-id="d3bfd-106">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>
- <span data-ttu-id="d3bfd-107">Tok posla je konfigurisan da šalje prilagođenu e-poruku za više od 200 korisnika po danu, više od 10.000 primalaca dnevno ili više od 30 poruka u minuti.</span><span class="sxs-lookup"><span data-stu-id="d3bfd-107">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>
- <span data-ttu-id="d3bfd-108">Kada pokrećete tok posla, e-poruka se ne šalje i primetićete sledeće ponašanje:</span><span class="sxs-lookup"><span data-stu-id="d3bfd-108">When you run the workflow, the email message isn't sent, and you notice the following behavior:</span></span>
    - <span data-ttu-id="d3bfd-109">Za tok posla koji koristi SharePoint 2013 platformu, potražite stranicu **Status toka posla** .</span><span class="sxs-lookup"><span data-stu-id="d3bfd-109">For a workflow using the SharePoint 2013 platform type, you browse to the **Workflow Status** page.</span></span> <span data-ttu-id="d3bfd-110">Na stranici "Status toka posla", **unutrašnji status** je podešen na **Početak**, a balončić sa informacijama **ne može da**se prikaže primaocu.</span><span class="sxs-lookup"><span data-stu-id="d3bfd-110">On the Workflow Status page, the **Internal Status** is set to **Started**, and the information balloon displays **Unable to send to a recipient**.</span></span>

<span data-ttu-id="d3bfd-111">Da biste rešili ovaj problem, konfigurišite tok posla da šalje e-poruke bez prekoračenja [ograničenja Exchange online pošiljaoca](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span><span class="sxs-lookup"><span data-stu-id="d3bfd-111">To work around this issue, configure your workflow to send email messages without exceeding the [Exchange Online sender limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span></span> <span data-ttu-id="d3bfd-112">Na primer, koristite pauzu u toku posla, pošaljite e-poruku Microsoft 365 grupi, grupi za distribuciju ili bezbednosnoj grupi sa omogućenom poštom ili pošaljite poruku manjim od 200 primalaca.</span><span class="sxs-lookup"><span data-stu-id="d3bfd-112">For example, use a pause in the workflow, send the email to a Microsoft 365 group, a distribution group or mail enabled security group, or send the message to fewer than 200 recipients at a time.</span></span>


<span data-ttu-id="d3bfd-113">Više informacija potražite u sledećem [članku](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).</span><span class="sxs-lookup"><span data-stu-id="d3bfd-113">For more information, see the following [article](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).</span></span>

## <a name="related-topics"></a><span data-ttu-id="d3bfd-114">Сродне теме</span><span class="sxs-lookup"><span data-stu-id="d3bfd-114">Related topics</span></span>
- [<span data-ttu-id="d3bfd-115">Kreiranje protoka</span><span class="sxs-lookup"><span data-stu-id="d3bfd-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="d3bfd-116">SharePoint i protok</span><span class="sxs-lookup"><span data-stu-id="d3bfd-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 