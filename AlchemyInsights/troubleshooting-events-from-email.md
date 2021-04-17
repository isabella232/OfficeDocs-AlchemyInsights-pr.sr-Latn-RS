---
title: Rešavanje problema sa događajima iz e-pošte
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
- "9000301"
- "5765"
ms.openlocfilehash: 2cea347f248a3b04873428946f1817657af04773
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/15/2021
ms.locfileid: "51834853"
---
# <a name="troubleshooting-events-from-email"></a><span data-ttu-id="ca224-102">Rešavanje problema sa događajima iz e-pošte</span><span class="sxs-lookup"><span data-stu-id="ca224-102">Troubleshooting Events from Email</span></span>

1. <span data-ttu-id="ca224-103">Provera da li je funkcija omogućena za poštansko sanduče: **Get-EventsFromEmailConfiguration -Identity <mailbox>**</span><span class="sxs-lookup"><span data-stu-id="ca224-103">Verify the feature is enabled for the mailbox: **Get-EventsFromEmailConfiguration -Identity <mailbox>**</span></span>

2. <span data-ttu-id="ca224-104">Zatim pogledajte evidenciju "Događaji iz **e-pošte" evidencije Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**</span><span class="sxs-lookup"><span data-stu-id="ca224-104">Then look at the 'Events from Email' logs **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**</span></span>

3. <span data-ttu-id="ca224-105">U evidencijama "Događaji iz e-pošte" pronađite InternetMessageId koji se podudara sa stavkom u poštanskom sandučetu.</span><span class="sxs-lookup"><span data-stu-id="ca224-105">In the 'Events from Email' logs, find the InternetMessageId that matches the item in the mailbox.</span></span>  

4. <span data-ttu-id="ca224-106">TrustScore određuje da li je stavka dodata ili ne.</span><span class="sxs-lookup"><span data-stu-id="ca224-106">The TrustScore determines if the item is added or not.</span></span> <span data-ttu-id="ca224-107">Događaji će se dodati samo ako je TrustScore = "Trusted".</span><span class="sxs-lookup"><span data-stu-id="ca224-107">Events will only be added if the TrustScore = "Trusted".</span></span>

<span data-ttu-id="ca224-108">Svojstva TrustScore određuju SPF, Dkim ili Dmarc svojstva koja se nalazi u zaglavlju poruke.</span><span class="sxs-lookup"><span data-stu-id="ca224-108">The TrustScore is determined by SPF, Dkim or Dmarc properties, which are in the Message Header.</span></span>

<span data-ttu-id="ca224-109">Da biste prikazali ova svojstva:</span><span class="sxs-lookup"><span data-stu-id="ca224-109">To view these properties:</span></span>

<span data-ttu-id="ca224-110">**Outlook za stone računare**</span><span class="sxs-lookup"><span data-stu-id="ca224-110">**Desktop Outlook**</span></span>

- <span data-ttu-id="ca224-111">Otvaranje stavke</span><span class="sxs-lookup"><span data-stu-id="ca224-111">Open the item</span></span>
- <span data-ttu-id="ca224-112">Svojstva datoteke > -> internet zaglavljima</span><span class="sxs-lookup"><span data-stu-id="ca224-112">File -> Properties -> Internet Headers</span></span>

<span data-ttu-id="ca224-113">ili</span><span class="sxs-lookup"><span data-stu-id="ca224-113">or</span></span>

<span data-ttu-id="ca224-114">**MFCMapi**</span><span class="sxs-lookup"><span data-stu-id="ca224-114">**MFCMapi**</span></span>

- <span data-ttu-id="ca224-115">Prelaženje do stavke u prijemnom poštanskom sandučetu</span><span class="sxs-lookup"><span data-stu-id="ca224-115">Navigate to the item in the inbox</span></span>
- <span data-ttu-id="ca224-116">Potraži PR_TRANSPORT_MESSAGE_HEADERS_W</span><span class="sxs-lookup"><span data-stu-id="ca224-116">Look for PR_TRANSPORT_MESSAGE_HEADERS_W</span></span>

<span data-ttu-id="ca224-117">Ova svojstva se određuju i zapisuju tokom prenosa i usućivanja.</span><span class="sxs-lookup"><span data-stu-id="ca224-117">These properties are determined and recorded during transport and routing.</span></span> <span data-ttu-id="ca224-118">Da biste dodatno rešavali probleme, možda ćete morati da pratite podršku za prenos o greškama u spF, DKIM i.ili DMARC-u.</span><span class="sxs-lookup"><span data-stu-id="ca224-118">For further troubleshooting, you may need to follow up with Transport Support about the failures in  SPF, DKIM and.or DMARC.</span></span>