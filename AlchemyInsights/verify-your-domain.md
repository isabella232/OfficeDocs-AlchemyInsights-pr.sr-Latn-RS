---
title: Verifikacija domena
ms.author: pebaum
author: pebaum
manager: scotv
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
ms.openlocfilehash: 4a34de7fa2aaaae365cf4562d31590d4b5fb7544
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/15/2021
ms.locfileid: "51771005"
---
# <a name="verify-your-domain"></a><span data-ttu-id="41ff1-102">Verifikacija domena</span><span class="sxs-lookup"><span data-stu-id="41ff1-102">Verify your domain</span></span>

 <span data-ttu-id="41ff1-103">**Zapis verovatno nije ažuriran na internetu.**</span><span class="sxs-lookup"><span data-stu-id="41ff1-103">**The record probably hasn't updated across the Internet.**</span></span>
  
<span data-ttu-id="41ff1-104">Obično je potrebno samo nekoliko minuta da vidimo novi zapis, ali ponekad je potrebno i do nekoliko časova.</span><span class="sxs-lookup"><span data-stu-id="41ff1-104">It typically only takes a few minutes for us to be able to see the new record, but occasionally it can take as long as a few hours.</span></span> 
  
- <span data-ttu-id="41ff1-105">Ako ste to već čekali, još jednom proverite da li ste kopirali i nalepili tačnu vrednost u TXT zapis verifikacije kod DNS hosta.</span><span class="sxs-lookup"><span data-stu-id="41ff1-105">If you've waited that long already, double-check that you've copied and pasted the exact value into the TXT verification record at your DNS host.</span></span> <span data-ttu-id="41ff1-106">Jedan uobičajeni problem je da nije obuhvaćeno deo "MS=" zapisa.</span><span class="sxs-lookup"><span data-stu-id="41ff1-106">One common issue is not including the "MS=" part of the record.</span></span> <span data-ttu-id="41ff1-107">I to nam je potrebno!</span><span class="sxs-lookup"><span data-stu-id="41ff1-107">We need that too!</span></span>

- <span data-ttu-id="41ff1-108">Na nekim DNS hostovima morate da pređete na dodatni korak za čuvanje datoteke zone (u kojoj je uskladišten DNS zapis) kako bi se ažurirao na internetu.</span><span class="sxs-lookup"><span data-stu-id="41ff1-108">At some DNS hosts, you have to take an extra step to save the zone file (where the DNS record is stored) so that it will update across the Internet.</span></span> <span data-ttu-id="41ff1-109">Uverite se da ste sačuvali promene kako bi Microsoft mogao da vidi i verifikuje zapis.</span><span class="sxs-lookup"><span data-stu-id="41ff1-109">Make sure you've saved your changes so Microsoft can see and verify the record.</span></span>
