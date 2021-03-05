---
title: O bezbednosnim ispravkama za Exchange Server
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9005482"
- "9005483"
- "9413"
- "9412"
ms.openlocfilehash: 87a5cf1ac4dfb96a5406f6b1431adb6ead074fd6
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/04/2021
ms.locfileid: "50482989"
---
# <a name="about-exchange-server-security-updates"></a><span data-ttu-id="4b5c1-102">O bezbednosnim ispravkama za Exchange Server</span><span class="sxs-lookup"><span data-stu-id="4b5c1-102">About Exchange Server Security updates</span></span>

<span data-ttu-id="4b5c1-103">Microsoft je objavio seriju ključnih bezbednosnih ispravki za Exchange server.</span><span class="sxs-lookup"><span data-stu-id="4b5c1-103">Microsoft has released a series of critical security updates for Exchange Server on-premises.</span></span> <span data-ttu-id="4b5c1-104">Verzije sa pogođene serverom su nivoi ažuriranja Exchange servera 2010, 2013, 2016 i 2019.</span><span class="sxs-lookup"><span data-stu-id="4b5c1-104">The affected server versions are any update levels of Exchange Server 2010, 2013, 2016 and 2019.</span></span> <span data-ttu-id="4b5c1-105">Exchange online nije uključen, ali ako imate neke lokalne Exchange servere zbog hibridne konfiguracije, oni su potencijalno ranjivi.</span><span class="sxs-lookup"><span data-stu-id="4b5c1-105">Exchange Online is NOT impacted, but if you have some on-premises Exchange servers due to Hybrid configuration, they are potentially vulnerable.</span></span>

<span data-ttu-id="4b5c1-106">Da biste ažurirali lokalno servere, moraćete da koristite najmanje sledeće verzije razmene:</span><span class="sxs-lookup"><span data-stu-id="4b5c1-106">To update your on-premises servers will have to be running at least the following versions of Exchange:</span></span>

- <span data-ttu-id="4b5c1-107">Exchange 2010 servisni paket 3</span><span class="sxs-lookup"><span data-stu-id="4b5c1-107">Exchange 2010 Service Pack 3</span></span>
- <span data-ttu-id="4b5c1-108">Exchange Server 2013 CU 23</span><span class="sxs-lookup"><span data-stu-id="4b5c1-108">Exchange Server 2013 CU 23</span></span>
- <span data-ttu-id="4b5c1-109">Exchange Server 2016 CU 19 ili CU 18</span><span class="sxs-lookup"><span data-stu-id="4b5c1-109">Exchange Server 2016 CU 19 or CU 18</span></span>
- <span data-ttu-id="4b5c1-110">Exchange Server 2019 CU 8 ili CU 7</span><span class="sxs-lookup"><span data-stu-id="4b5c1-110">Exchange Server 2019 CU 8 or CU 7</span></span>

<span data-ttu-id="4b5c1-111">Pogledajte sledeću objavu za lokaciju ispravki: [Izdato: mart 2021 Exchange Server Security Update](https://techcommunity.microsoft.com/t5/exchange-team-blog/released-march-2021-exchange-server-security-updates/ba-p/2175901)</span><span class="sxs-lookup"><span data-stu-id="4b5c1-111">Please see the following announcement for location of fixes: [Released: March 2021 Exchange Server Security Updates](https://techcommunity.microsoft.com/t5/exchange-team-blog/released-march-2021-exchange-server-security-updates/ba-p/2175901)</span></span>

<span data-ttu-id="4b5c1-112">**Važne beleške:**</span><span class="sxs-lookup"><span data-stu-id="4b5c1-112">**Important notes:**</span></span>

<span data-ttu-id="4b5c1-113">Instalacija ispravki neće funkcionisati ako lokalni serveri ne izvršavaju potrebne Exchange verzije, na listi gorenavedenih.</span><span class="sxs-lookup"><span data-stu-id="4b5c1-113">Installation of updates will not work if your on-premises servers are not running required Exchange versions, as per the above list.</span></span>

<span data-ttu-id="4b5c1-114">Ako ručno instalirate ispravke, pročitajte odeljak "poznati problemi" u člancima ispravki baze znanja za važne informacije.</span><span class="sxs-lookup"><span data-stu-id="4b5c1-114">If installing updates manually, please read the "Known issues" section of update KB articles for important information.</span></span> <span data-ttu-id="4b5c1-115">Bezbednosne ispravke moraju da se pokrenu sa poviљene CMD/PowerShell odziv!</span><span class="sxs-lookup"><span data-stu-id="4b5c1-115">Security updates MUST be run from elevated CMD/PowerShell prompt!</span></span>
