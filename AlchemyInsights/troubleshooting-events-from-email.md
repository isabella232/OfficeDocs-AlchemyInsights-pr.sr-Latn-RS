---
title: Rešavanje problema sa e-poštom
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000301"
- "5765"
ms.openlocfilehash: e27589b7f6730036040b948b6275cef072fd8235
ms.sourcegitcommit: dc149ab45fbc2c974b54fb81156d2bc1b07017bb
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 06/02/2020
ms.locfileid: "44569405"
---
# <a name="troubleshooting-events-from-email"></a><span data-ttu-id="913d7-102">Rešavanje problema sa e-poštom</span><span class="sxs-lookup"><span data-stu-id="913d7-102">Troubleshooting Events from Email</span></span>

1. <span data-ttu-id="913d7-103">Proverite da li je omogućena funkcija za poštansko sanduče: **get-Eventsfromemailiskonfiguracija <mailbox> -identitet**</span><span class="sxs-lookup"><span data-stu-id="913d7-103">Verify the feature is enabled for the mailbox: **Get-EventsFromEmailConfiguration -Identity <mailbox>**</span></span>

2. <span data-ttu-id="913d7-104">Zatim pogledajte ' događaje iz e-maila ' evidencije **Export-MailboxDiagnosticLogs <mailbox> -Component time profil**</span><span class="sxs-lookup"><span data-stu-id="913d7-104">Then look at the 'Events from Email' logs **Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**</span></span>

3. <span data-ttu-id="913d7-105">U "događajima iz evidencije e-pošte", pronađite Internetporuku koja se podudara sa stavkom u poštanskom sandučetu.</span><span class="sxs-lookup"><span data-stu-id="913d7-105">In the 'Events from Email' logs, find the InternetMessageId that matches the item in the mailbox.</span></span>  

4. <span data-ttu-id="913d7-106">Rezultat Pover, određuje da li je artikal dodat ili ne.</span><span class="sxs-lookup"><span data-stu-id="913d7-106">The TrustScore determines if the item is added or not.</span></span> <span data-ttu-id="913d7-107">Događaji će biti dodati samo ako je poverljiv rezultat = "pouzdan".</span><span class="sxs-lookup"><span data-stu-id="913d7-107">Events will only be added if the TrustScore = "Trusted".</span></span>

<span data-ttu-id="913d7-108">Rezultat povernje je određen svojstvima SPF, Dkim ili Dmark, koji se nalaze u zaglavlju poruke.</span><span class="sxs-lookup"><span data-stu-id="913d7-108">The TrustScore is determined by SPF, Dkim or Dmarc properties, which are in the Message Header.</span></span>

<span data-ttu-id="913d7-109">Da biste prikazali ova svojstva:</span><span class="sxs-lookup"><span data-stu-id="913d7-109">To view these properties:</span></span>

<span data-ttu-id="913d7-110">**Radnu površinu Outlook**</span><span class="sxs-lookup"><span data-stu-id="913d7-110">**Desktop Outlook**</span></span>

- <span data-ttu-id="913d7-111">Otvorite stavku</span><span class="sxs-lookup"><span data-stu-id="913d7-111">Open the item</span></span>
- <span data-ttu-id="913d7-112">Svojstva > datoteke-> Internet zaglavlja</span><span class="sxs-lookup"><span data-stu-id="913d7-112">File -> Properties -> Internet Headers</span></span>

<span data-ttu-id="913d7-113">Ili</span><span class="sxs-lookup"><span data-stu-id="913d7-113">or</span></span>

<span data-ttu-id="913d7-114">**MFCMapi**</span><span class="sxs-lookup"><span data-stu-id="913d7-114">**MFCMapi**</span></span>

- <span data-ttu-id="913d7-115">Kretanje do stavke u prijemnom poštanskom sandučetu</span><span class="sxs-lookup"><span data-stu-id="913d7-115">Navigate to the item in the inbox</span></span>
- <span data-ttu-id="913d7-116">Potraži PR_TRANSPORT_MESSAGE_HEADERS_W</span><span class="sxs-lookup"><span data-stu-id="913d7-116">Look for PR_TRANSPORT_MESSAGE_HEADERS_W</span></span>

<span data-ttu-id="913d7-117">Ova svojstva se određuju i zapisuju tokom transporta i proizvodnog postupka.</span><span class="sxs-lookup"><span data-stu-id="913d7-117">These properties are determined and recorded during transport and routing.</span></span> <span data-ttu-id="913d7-118">Za dalje rešavanje problema, možda ćete morati da pratite podršku za transport u vezi sa otkazima u SPF-u, DKIM i. ili DMARK.</span><span class="sxs-lookup"><span data-stu-id="913d7-118">For further troubleshooting, you may need to follow up with Transport Support about the failures in  SPF, DKIM and.or DMARC.</span></span>