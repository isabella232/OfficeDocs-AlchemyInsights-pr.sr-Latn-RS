---
title: Primenjivanje najboljih praksi za napredne lovačke upite
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: cd13e2e8801db3df91140ce371813d900d72e38b
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/11/2021
ms.locfileid: "50749547"
---
# <a name="apply-best-practices-for-advanced-hunting-queries"></a><span data-ttu-id="0df40-102">Primenjivanje najboljih praksi za napredne lovačke upite</span><span class="sxs-lookup"><span data-stu-id="0df40-102">Apply best practices for advanced hunting queries</span></span>

<span data-ttu-id="0df40-103">Da biste brže pokrenuli rezultate i izbegli vremenska ograničenja prilikom pokretanja složenih upita, primene ove najbolje prakse:</span><span class="sxs-lookup"><span data-stu-id="0df40-103">To get results faster and to avoid timeouts while running complex queries, apply these best practices:</span></span>

- <span data-ttu-id="0df40-104">Prilikom pokušaja novih upita, uvek koristite limit da biste izbegli izuzetno velike skupove ishoda.</span><span class="sxs-lookup"><span data-stu-id="0df40-104">When trying new queries, always use a limit, to avoid getting extremely large result sets.</span></span> <span data-ttu-id="0df40-105">Pored toga, koristite `count` ga da biste napravili inicijalnu procenu veličine skupa ishoda.</span><span class="sxs-lookup"><span data-stu-id="0df40-105">Also, use `count` to make an initial assessment of the result set's size.</span></span>
- <span data-ttu-id="0df40-106">Najpre koristite vremenske filtere.</span><span class="sxs-lookup"><span data-stu-id="0df40-106">Use time filters first.</span></span> <span data-ttu-id="0df40-107">Idealno, ograničite upite na sedam dana.</span><span class="sxs-lookup"><span data-stu-id="0df40-107">Ideally, limit your queries to seven days.</span></span>
- <span data-ttu-id="0df40-108">Na početku upita, odmah posle filtera vremena, dodajte filtere za koje se očekuje da će ukloniti većinu podataka.</span><span class="sxs-lookup"><span data-stu-id="0df40-108">In the beginning of a query, right after the time filter, add the filters expected to remove most of the data.</span></span>
- <span data-ttu-id="0df40-109">Kada tražite pune simbole, koristite `has` operator umesto `contains` .</span><span class="sxs-lookup"><span data-stu-id="0df40-109">When looking for full tokens, use the `has` operator rather than `contains`.</span></span>
- <span data-ttu-id="0df40-110">Pokrećete pretragu u određenoj koloni, a ne u svim kolonama.</span><span class="sxs-lookup"><span data-stu-id="0df40-110">Run a search on a specific column rather than across all columns.</span></span>
- <span data-ttu-id="0df40-111">Prilikom pridruživanja tabelama, prvo navedite tabelu sa manje redova.</span><span class="sxs-lookup"><span data-stu-id="0df40-111">When joining tables, first specify the table with fewer rows.</span></span>
- <span data-ttu-id="0df40-112">`project` Samo neophodne kolone iz tabela kojima ste se pridružili.</span><span class="sxs-lookup"><span data-stu-id="0df40-112">`project` only the necessary columns from the tables you've joined.</span></span>

<span data-ttu-id="0df40-113">Da biste saznali više, pogledajte članak [Napredni osnovni načini za lov Query](https://go.microsoft.com/fwlink/?linkid=2144812).</span><span class="sxs-lookup"><span data-stu-id="0df40-113">To learn more, see [Advanced hunting query best practices](https://go.microsoft.com/fwlink/?linkid=2144812).</span></span>
