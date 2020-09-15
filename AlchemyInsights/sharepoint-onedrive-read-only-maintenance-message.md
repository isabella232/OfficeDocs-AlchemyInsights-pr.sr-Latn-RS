---
title: Samo za čitanje kada pokušate da koristite SharePoint ili OneDrive
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "127"
- "128"
ms.assetid: de7b6877-f3f9-4402-8072-c73783aaccaa
ms.openlocfilehash: a3d313816beefcefa4d93528d3ad9a684e60390e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670846"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a><span data-ttu-id="40792-102">Samo za čitanje kada pokušate da koristite SharePoint ili OneDrive</span><span class="sxs-lookup"><span data-stu-id="40792-102">Read-Only for Maintenance message when attempting to use SharePoint or OneDrive</span></span>

<span data-ttu-id="40792-103">Korisnici mogu primati poruku **o održavanju samo za čitanje** kada pokušaju da koriste SharePoint ili OneDrive za neki od sledećih scenarija.</span><span class="sxs-lookup"><span data-stu-id="40792-103">Users may receive a **Read-Only for Maintenance** message when attempting to use SharePoint or OneDrive for one of the following scenarios.</span></span> 

-   <span data-ttu-id="40792-104">Planirana ili aktivna aktivnost održavanja.</span><span class="sxs-lookup"><span data-stu-id="40792-104">A planned or active maintenance activity.</span></span>  <span data-ttu-id="40792-105">Potražite ih tako što ćete se u [centru za poruke](https://portal.office.com/adminportal/home#/messagecenter).</span><span class="sxs-lookup"><span data-stu-id="40792-105">Check for them by navigating to the [Message Center](https://portal.office.com/adminportal/home#/messagecenter).</span></span>
-   <span data-ttu-id="40792-106">Događaj visokog prioriteta, aktivni servisni problem koji se možda dešava.</span><span class="sxs-lookup"><span data-stu-id="40792-106">A high-priority, active service incident that may be occurring.</span></span> <span data-ttu-id="40792-107">Provjerite da li postoje savjeri/incidenti tako što ćete se usmeriti na [uslugu usluge](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="40792-107">Check for any advisories/incidents by navigating to [Service Health](https://portal.office.com/adminportal/home#/servicehealth).</span></span>
-   <span data-ttu-id="40792-108">Međuverski scenario oporavka koji se može dogoditi zbog bilo kog neočekivanog događaja na serverima koji bi mogli da traju manje od 30 minuta ili tako nesto.</span><span class="sxs-lookup"><span data-stu-id="40792-108">A minor auto-healing recovery scenario that could be happening due to any unexpected events on the servers which might last for less than 30 min or so.</span></span> 
    
    <span data-ttu-id="40792-109">Ne postoje centar za poruke ili zdravstvene objave usluge za ova mala oporavka, ali trebalo bi da se brzo vratite u normalu.</span><span class="sxs-lookup"><span data-stu-id="40792-109">There are no Message Center or Service Health posts for these minor recoveries but you should be back to normal very soon.</span></span>

<span data-ttu-id="40792-110">U vrlo nekoliko navrata primećeni smo da je jedan od tri scenarija navedena u navedenom delu i da je usluga vraćena u prethodno stanje, ali keš korisnika pregledača nije očistljen.</span><span class="sxs-lookup"><span data-stu-id="40792-110">On very few occasions we observed that one of the three scenarios listed above have been the cause, and service has been restored, but the users browser cache hasn’t been cleared up.</span></span>

<span data-ttu-id="40792-111">Pokušajte da obrišite keš pregledača pre nego što se vratite na stranicu.</span><span class="sxs-lookup"><span data-stu-id="40792-111">Please attempt to clear the browser cache before navigating to the site.</span></span>

1. <span data-ttu-id="40792-112">U Microsoft pregledaču Edge izaberite stavku **Postavke**, a zatim izaberite stavku **privatnost i bezbednost**.</span><span class="sxs-lookup"><span data-stu-id="40792-112">In your Microsoft Edge browser, select **Settings**, and then select **Privacy and Security**.</span></span>
2. <span data-ttu-id="40792-113">U okviru **Izbriši pregledanje**izaberite **stavku odaberite šta da obrišete**.</span><span class="sxs-lookup"><span data-stu-id="40792-113">Under **Clear browsing**, select **Choose what to clear**.</span></span>
3. <span data-ttu-id="40792-114">Izaberite stavku **kolačići i sačuvani podaci o Veb lokaciji**i izaberite stavku **čisti**.</span><span class="sxs-lookup"><span data-stu-id="40792-114">Select **Cookies and saved website data**, and select **Clear**.</span></span>

>[!Note] 
> <span data-ttu-id="40792-115">Ovi koraci mogu da se razlikuju kada koristite druge pregledače kao što je Mozilla Firefox ili Google Chrome.</span><span class="sxs-lookup"><span data-stu-id="40792-115">These steps may differ when using other browsers such as Mozilla Firefox or Google Chrome.</span></span>

>[!Note] 
> <span data-ttu-id="40792-116">Druga opcija bi bila da otvorite SharePoint sajt ili OneDrive u novom InPrivate prozoru.</span><span class="sxs-lookup"><span data-stu-id="40792-116">Another option would be to open your SharePoint site or OneDrive in a new InPrivate window.</span></span>