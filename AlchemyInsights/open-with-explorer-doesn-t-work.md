---
title: Otvaranje pomoću programa Explorer ne radi
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: 5bf28982533d8ca9998605cf3592f317c0ef99b0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47694470"
---
# <a name="open-with-explorer-isnt-working"></a><span data-ttu-id="bf2c2-102">Otvori pomoću programa Explorer ne radi</span><span class="sxs-lookup"><span data-stu-id="bf2c2-102">Open with Explorer isn't working</span></span>

<span data-ttu-id="bf2c2-103">Ako se **Otvori pomoću programa Explorer** ili **View u istraživaču datoteka** ne radi, uverite se da je usluga webklijenta podešena da **radi** tako što će pratiti dolenavedene korake.</span><span class="sxs-lookup"><span data-stu-id="bf2c2-103">If **Open with Explorer** or **View in File Explorer** doesn't work make sure the WebClient service is set to **Running** by following the steps below.</span></span> <span data-ttu-id="bf2c2-104">Na primer, možda će biti potrebno dugo vremena da se otvori SharePoint ili OneDrive biblioteka kada usluga nije pokrenuta.</span><span class="sxs-lookup"><span data-stu-id="bf2c2-104">For example, it might take a long time to open a SharePoint or OneDrive library when the service is not running.</span></span> 
  
1. <span data-ttu-id="bf2c2-105">U polju Windows pretraga otkucajte funkcija Run, izaberite stavku pokreće aplikaciju za računare, otkucajte usluge. msc, a zatim izaberite stavku **ENTER**.</span><span class="sxs-lookup"><span data-stu-id="bf2c2-105">In the Windows search box, type run, select the Run desktop app, type services.msc, and then select **Enter**.</span></span>
    
2. <span data-ttu-id="bf2c2-106">Pomerajte se nadole do usluge Webklijenta i potvrdite izbor u polju za proveru **statusa** .</span><span class="sxs-lookup"><span data-stu-id="bf2c2-106">Scroll down to the WebClient service and check the **Status** column.</span></span> <span data-ttu-id="bf2c2-107">Ako status usluge Webklenta nije **pokrenut**, kliknite dvaput na uslugu, kliknite na dugme **Start**, a zatim kliknite na dugme **u redu**.</span><span class="sxs-lookup"><span data-stu-id="bf2c2-107">If the WebClient service status is not **Running**, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="bf2c2-108">Omogućite uslugu, ako je potrebno, tako što ćete izabrati stavku **ručno** ili **automatski** u polju **Tip pokretanja** .</span><span class="sxs-lookup"><span data-stu-id="bf2c2-108">Enable the service, if needed, by selecting either **Manual** or **Automatic** in the **Startup type** box.</span></span> 
    
> [!NOTE]
> <span data-ttu-id="bf2c2-109">Da biste rešili probleme prilikom otvaranja u istraživaču datoteka, pogledajte članak [Otvaranje u programu Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span><span class="sxs-lookup"><span data-stu-id="bf2c2-109">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="bf2c2-110">Istražite sinhronizaciju kao bolju alternativu: [Sinhronizovanje SharePoint datoteka sa novim OneDrive klijentom za sinhronizaciju](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="bf2c2-110">Explore sync as a better alternative: [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span> 
  

