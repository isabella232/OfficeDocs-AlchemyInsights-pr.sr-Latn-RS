---
title: Grafikon prikazuje različit broj zapisa u koordinatnoj mreži
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5611"
- "9002930"
ms.openlocfilehash: 3d0be28c783bb129d05484565c6c2a56ac5e0acf
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439964"
---
# <a name="chart-shows-different-number-of-records-in-grid"></a><span data-ttu-id="4f515-102">Grafikon prikazuje različit broj zapisa u koordinatnoj mreži</span><span class="sxs-lookup"><span data-stu-id="4f515-102">Chart shows different number of records in grid</span></span>

<span data-ttu-id="4f515-103">**Simptoma**</span><span class="sxs-lookup"><span data-stu-id="4f515-103">**Symptom**</span></span>

<span data-ttu-id="4f515-104">Na stranici "grafikon na kontrolnoj tabli", kada kliknete na grafikon "..." i kliknite na dugme "Prikaži zapise", krećite se do stranice koordinatne mreže da biste videli sve zapise. Ponekad se broj zapisa menja.</span><span class="sxs-lookup"><span data-stu-id="4f515-104">For chart on dashboard page, when you click on chart "…" and click "View records", you navigate to grid page to see all the records.Sometimes, the number of records changes.</span></span>

<span data-ttu-id="4f515-105">**Izazvati**</span><span class="sxs-lookup"><span data-stu-id="4f515-105">**Cause**</span></span>

<span data-ttu-id="4f515-106">To je zbog razlike prikaza između grafikona na originalnoj stranici kontrolne table i grafikona na matičnoj stranici koordinatne mreže.</span><span class="sxs-lookup"><span data-stu-id="4f515-106">This is due to the difference of views between the chart on the original dashboard page and the chart on the grid home page.</span></span>  

<span data-ttu-id="4f515-107">**Rešenje**</span><span class="sxs-lookup"><span data-stu-id="4f515-107">**Solution**</span></span>

1. <span data-ttu-id="4f515-108">Proverite prikaz sa originalne stranice i prikaz u koordinatnoj mreži da biste videli da li se razlikuju.</span><span class="sxs-lookup"><span data-stu-id="4f515-108">Check the view from the original page and the view in the grid to see if they are different.</span></span>
2. <span data-ttu-id="4f515-109">Promenite prikaz u koordinatnoj mreži da bi se podudarali sa prikazom na originalnoj stranici.</span><span class="sxs-lookup"><span data-stu-id="4f515-109">Change the view in grid to match the view in the original page.</span></span>
3. <span data-ttu-id="4f515-110">Ako nije moguće pronaći ispravan prikaz, to obično znači da prikaz nije omogućen u dizajneru aplikacija.</span><span class="sxs-lookup"><span data-stu-id="4f515-110">If the correct view cannot be found, usually it means the view is not enabled in app designer.</span></span>
4. <span data-ttu-id="4f515-111">Idite na dizajner aplikacije određene aplikacije, odaberite entitet i njegove prikaze, proverite prikaz koji želite da omogućite, sačuvajte, objavite i zatvorite.</span><span class="sxs-lookup"><span data-stu-id="4f515-111">Go to app designer of the specific app, choose the entity and its views, check the view you want to enable, save, publish and close.</span></span>
5. <span data-ttu-id="4f515-112">Osvežite stranicu.</span><span class="sxs-lookup"><span data-stu-id="4f515-112">Refresh the page.</span></span>