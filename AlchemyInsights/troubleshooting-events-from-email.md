---
title: Rešavanje problema sa e-poštom
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000301"
- "5765"
ms.openlocfilehash: 9efd969e3e639c2679b0768c4a0fd045916b00d1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658748"
---
# <a name="troubleshooting-events-from-email"></a><span data-ttu-id="824bf-102">Rešavanje problema sa e-poštom</span><span class="sxs-lookup"><span data-stu-id="824bf-102">Troubleshooting Events from Email</span></span>

1. <span data-ttu-id="824bf-103">Potvrdite da je funkcija omogućena za poštansko sanduče: **da biste dobili-Eventsfromemail Configuration <mailbox> – identitet**</span><span class="sxs-lookup"><span data-stu-id="824bf-103">Verify the feature is enabled for the mailbox: **Get-EventsFromEmailConfiguration -Identity <mailbox>**</span></span>

2. <span data-ttu-id="824bf-104">Zatim pogledajte "događaji iz e-pošte" evidentira **Export-Mailboxdijagnostičke zapise <mailbox> – vremenski profil komponente**</span><span class="sxs-lookup"><span data-stu-id="824bf-104">Then look at the 'Events from Email' logs **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**</span></span>

3. <span data-ttu-id="824bf-105">U evidenciji "događaji iz e-pošte" Pronađite aplikaciju Internegeid koja se podudara sa stavkom u poštanskom sandučetu.</span><span class="sxs-lookup"><span data-stu-id="824bf-105">In the 'Events from Email' logs, find the InternetMessageId that matches the item in the mailbox.</span></span>  

4. <span data-ttu-id="824bf-106">Vrednost "pouzdanost" određuje da li se stavka dodaje ili ne.</span><span class="sxs-lookup"><span data-stu-id="824bf-106">The TrustScore determines if the item is added or not.</span></span> <span data-ttu-id="824bf-107">Događaji će biti dodati samo ako je vrednost "Pouzdani" = "pouzdan".</span><span class="sxs-lookup"><span data-stu-id="824bf-107">Events will only be added if the TrustScore = "Trusted".</span></span>

<span data-ttu-id="824bf-108">Vrednost "pouzdanost" određuje SPF, Dkim ili Dmark svojstva koja se nalaze u zaglavlju poruke.</span><span class="sxs-lookup"><span data-stu-id="824bf-108">The TrustScore is determined by SPF, Dkim or Dmarc properties, which are in the Message Header.</span></span>

<span data-ttu-id="824bf-109">Da biste prikazali ova svojstva:</span><span class="sxs-lookup"><span data-stu-id="824bf-109">To view these properties:</span></span>

<span data-ttu-id="824bf-110">**Outlook za stone računare**</span><span class="sxs-lookup"><span data-stu-id="824bf-110">**Desktop Outlook**</span></span>

- <span data-ttu-id="824bf-111">Otvaranje stavke</span><span class="sxs-lookup"><span data-stu-id="824bf-111">Open the item</span></span>
- <span data-ttu-id="824bf-112">Svojstva >-> Internet zaglavlja</span><span class="sxs-lookup"><span data-stu-id="824bf-112">File -> Properties -> Internet Headers</span></span>

<span data-ttu-id="824bf-113">Jer</span><span class="sxs-lookup"><span data-stu-id="824bf-113">or</span></span>

<span data-ttu-id="824bf-114">**MFCMapi**</span><span class="sxs-lookup"><span data-stu-id="824bf-114">**MFCMapi**</span></span>

- <span data-ttu-id="824bf-115">Idite do stavke u prijemnom poštanskom sandučetu</span><span class="sxs-lookup"><span data-stu-id="824bf-115">Navigate to the item in the inbox</span></span>
- <span data-ttu-id="824bf-116">Potražite PR_TRANSPORT_MESSAGE_HEADERS_W</span><span class="sxs-lookup"><span data-stu-id="824bf-116">Look for PR_TRANSPORT_MESSAGE_HEADERS_W</span></span>

<span data-ttu-id="824bf-117">Ova svojstva su rešena i snimljena tokom transporta i proizvodnog postupka.</span><span class="sxs-lookup"><span data-stu-id="824bf-117">These properties are determined and recorded during transport and routing.</span></span> <span data-ttu-id="824bf-118">Da biste mogli da rešite problem, možda ćete morati da izvršite pretraživanje sa podrškom za transport o neuspesima u programu SPF, DKIM i. ili DMARK.</span><span class="sxs-lookup"><span data-stu-id="824bf-118">For further troubleshooting, you may need to follow up with Transport Support about the failures in  SPF, DKIM and.or DMARC.</span></span>