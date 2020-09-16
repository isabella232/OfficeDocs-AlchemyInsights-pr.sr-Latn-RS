---
title: Verifikacija domena
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "47"
- "48"
- "8"
ms.assetid: 81fd176b-3d67-4e52-9ab8-d36602412734
ms.openlocfilehash: d30f9b51c0164acd126f214a581ad6cec5eec04e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47734320"
---
# <a name="verify-your-domain"></a><span data-ttu-id="61483-102">Verifikacija domena</span><span class="sxs-lookup"><span data-stu-id="61483-102">Verify your domain</span></span>

 <span data-ttu-id="61483-103">**Zapis se verovatno ne ažurira preko interneta.**</span><span class="sxs-lookup"><span data-stu-id="61483-103">**The record probably hasn't updated across the Internet.**</span></span>
  
<span data-ttu-id="61483-104">Obično je potrebno samo nekoliko minuta da vidimo novi zapis, ali povremeno može da potraje nekoliko časova.</span><span class="sxs-lookup"><span data-stu-id="61483-104">It typically only takes a few minutes for us to be able to see the new record, but occasionally it can take as long as a few hours.</span></span> 
  
- <span data-ttu-id="61483-105">Ako ste tako dugo čekali, ponovo proverite da li ste kopirali i nalepili tačnu vrednost u TXT zapis verifikacije u DNS host.</span><span class="sxs-lookup"><span data-stu-id="61483-105">If you've waited that long already, double-check that you've copied and pasted the exact value into the TXT verification record at your DNS host.</span></span> <span data-ttu-id="61483-106">Jedan uobičajeni problem nije deo zapisa "MS =".</span><span class="sxs-lookup"><span data-stu-id="61483-106">One common issue is not including the "MS=" part of the record.</span></span> <span data-ttu-id="61483-107">I to nam treba!</span><span class="sxs-lookup"><span data-stu-id="61483-107">We need that too!</span></span>

- <span data-ttu-id="61483-108">Na neki DNS host, morate da izvršite dodatni stepenik da biste sačuvali datoteku zone (gde je uskladišten DNS zapis) tako da se ažurira na internetu.</span><span class="sxs-lookup"><span data-stu-id="61483-108">At some DNS hosts, you have to take an extra step to save the zone file (where the DNS record is stored) so that it will update across the Internet.</span></span> <span data-ttu-id="61483-109">Uverite se da ste sačuvali promene tako da Microsoft može da vidi i potvrdi zapis.</span><span class="sxs-lookup"><span data-stu-id="61483-109">Make sure you've saved your changes so Microsoft can see and verify the record.</span></span>
