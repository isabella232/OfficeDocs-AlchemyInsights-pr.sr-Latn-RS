---
title: Rešavanje problema pomoću funkcije "Otvori pomoću programa Explorer"
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
ms.assetid: ed852342-e33f-4450-8400-63d30df09476
ms.openlocfilehash: e7fe59b94d216d89c2f2f7100a3d8bf7a0b0196e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47659072"
---
# <a name="fix-problems-with-open-with-explorer"></a><span data-ttu-id="698e3-102">Rešavanje problema sa otvorenim programom Explorer</span><span class="sxs-lookup"><span data-stu-id="698e3-102">Fix problems with Open with Explorer</span></span>

<span data-ttu-id="698e3-103">Rešite uobičajene probleme sa otvaranjem biblioteke dokumenata u sistemu SharePoint ili OneDrive pomoću komande " **Otvori pomoću programa Explorer** ":</span><span class="sxs-lookup"><span data-stu-id="698e3-103">Fix common problems with opening a document library in SharePoint or OneDrive using the **Open with Explorer** command:</span></span> 
  
- <span data-ttu-id="698e3-104">Koristite Internet Explorer 10 ili Internet Explorer 11.</span><span class="sxs-lookup"><span data-stu-id="698e3-104">Use Internet Explorer 10 or Internet Explorer 11.</span></span> <span data-ttu-id="698e3-105">**Otvori pomoću programa Explorer** nije kompatibilan sa Microsoft Edge, Google Chrome, Firefox i drugima.</span><span class="sxs-lookup"><span data-stu-id="698e3-105">**Open with Explorer** isn't compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="698e3-106">**Otvaranje pomoću pregledača** je onemogućiti u svim pregledačima osim u programu Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="698e3-106">**Open with Explorer** is disabled in all browsers except Internet Explorer.</span></span> 
    
- <span data-ttu-id="698e3-107">**Otvori pomoću programa Explorer** nije dostupan u modernom iskustvu za SharePoint biblioteke.</span><span class="sxs-lookup"><span data-stu-id="698e3-107">**Open with Explorer** is not available in the modern experience for SharePoint libraries.</span></span> <span data-ttu-id="698e3-108">Umesto toga koristite **prikaz u istraživaču datoteka** .</span><span class="sxs-lookup"><span data-stu-id="698e3-108">Use **View in File Explorer** instead.</span></span> <span data-ttu-id="698e3-109">Izaberite stavku **Opcije prikaza** \> **u istraživaču datoteka**.</span><span class="sxs-lookup"><span data-stu-id="698e3-109">Select **View options** \> **View in File Explorer**.</span></span> <span data-ttu-id="698e3-110">Prikaz u istraživaču datoteka nije kompatibilan sa aplikacijom Microsoft Edge, Google Chrome, Firefox i drugima.</span><span class="sxs-lookup"><span data-stu-id="698e3-110">View in File Explorer is not compatible with Microsoft Edge, Google Chrome, Firefox and others.</span></span> <span data-ttu-id="698e3-111">**Prikaz u istraživaču datoteka** je dostupan samo u programu Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="698e3-111">**View in File Explorer** in available only in Internet Explorer.</span></span> 
    
- <span data-ttu-id="698e3-112">Proverite da li je pokrenuta usluga Webklijenta.</span><span class="sxs-lookup"><span data-stu-id="698e3-112">Make sure the WebClient service is running.</span></span> <span data-ttu-id="698e3-113">U polju Windows pretraga otkucajte funkcija Run, izaberite stavku pokreće aplikaciju za računare, otkucajte usluge. msc, a zatim pritisnite taster ENTER.</span><span class="sxs-lookup"><span data-stu-id="698e3-113">In the Windows search box, type run, select the Run desktop app, type services.msc, and then press Enter.</span></span> <span data-ttu-id="698e3-114">Pomerajte se nadole do usluge Webklijenta i uverite se da kolona **statusa** prikazuje "pokretanje".</span><span class="sxs-lookup"><span data-stu-id="698e3-114">Scroll down to the WebClient service and make sure the **Status** column displays "Running."</span></span> <span data-ttu-id="698e3-115">Ako nije, kliknite dvaput na uslugu, kliknite na dugme **Start**, a zatim kliknite na dugme **u redu**.</span><span class="sxs-lookup"><span data-stu-id="698e3-115">If it doesn't, double-click the service, click **Start**, and then click **OK**.</span></span> <span data-ttu-id="698e3-116">(Možda ćete prvo morati da omogućite uslugu tako što ćete izabrati stavku **ručno** ili **automatski** u polju **Tip pokretanja** .)</span><span class="sxs-lookup"><span data-stu-id="698e3-116">(You might need to first enable the service by selecting either **Manual** or **Automatic** in the **Startup type** box.)</span></span> 
    
> [!NOTE]
> <span data-ttu-id="698e3-117">Otvaranje biblioteke u istraživaču datoteka je korisno ako jednom treba da kopirate ili premestite više datoteka i fascikli, ali ako želite da redovno radite u biblioteci, preporučujemo da je sinhronizuju.</span><span class="sxs-lookup"><span data-stu-id="698e3-117">Opening a library in File Explorer is handy if you need to copy or move multiple files and folders once, but if you want to regularly work in the library, we recommend syncing it.</span></span> <span data-ttu-id="698e3-118">Da biste rešili probleme prilikom otvaranja u istraživaču datoteka, pogledajte članak [Otvaranje u programu Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span><span class="sxs-lookup"><span data-stu-id="698e3-118">To troubleshoot issues opening in File Explorer, see [Open in Explorer](https://go.microsoft.com/fwlink/?linkid=871665).</span></span> <span data-ttu-id="698e3-119">Informacije o podešavanju sinhronizacije potražite [u članku sinhronizovanje SharePoint datoteka sa novim OneDrive klijentom za sinhronizaciju](https://go.microsoft.com/fwlink/?linkid=871666).</span><span class="sxs-lookup"><span data-stu-id="698e3-119">For info about setting up sync, see [Sync SharePoint files with the new OneDrive sync client](https://go.microsoft.com/fwlink/?linkid=871666).</span></span>
  
<span data-ttu-id="698e3-120">Pročitajte članak [Kako da koristite komandu "Otvori pomoću Explorera" da biste dobili dodatne informacije o rešavanju problema u sistemu SharePoint online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) .</span><span class="sxs-lookup"><span data-stu-id="698e3-120">Please see the article [How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) for more information.</span></span> 
  

