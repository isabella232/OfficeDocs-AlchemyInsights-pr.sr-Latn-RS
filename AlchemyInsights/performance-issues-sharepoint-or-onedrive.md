---
title: Problemi sa performansama – SharePoint ili OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1133"
- "2397"
- "2418"
- "5200018"
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 28867b71df5353dcee5cc3361742f10357a0efe1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771915"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a><span data-ttu-id="9cca8-102">SharePoint ili OneDrive spori, nedostupni ili nedostupni za više korisnika</span><span class="sxs-lookup"><span data-stu-id="9cca8-102">SharePoint or OneDrive slow, inaccessible, or unavailable for multiple users</span></span>

<span data-ttu-id="9cca8-103">SharePoint ili OneDrive mogu biti spori, nedostupni ili nedostupni, ili mogu da prikažu usluge nedostupne ili 503 grešaka, iz nekoliko razloga:</span><span class="sxs-lookup"><span data-stu-id="9cca8-103">SharePoint or OneDrive may be slow, inaccessible, or unavailable, or may display service unavailable or 503 errors, for several reasons:</span></span>
  
- <span data-ttu-id="9cca8-104">Ako je SharePoint ili OneDrive lokacija spora ili odložena za više korisnika, možda može postojati privremeni problem pri uslugama gde korisnici doživljaju povremene kašnjenja ili greške navigacije prilikom pristupanja SharePoint lokacijama ili OneDrive sadržaju.</span><span class="sxs-lookup"><span data-stu-id="9cca8-104">If your SharePoint or OneDrive site is slow or delayed for multiple users, there may be a temporary service issue where users experience intermittent delays or navigation errors when accessing SharePoint sites or OneDrive content.</span></span> <span data-ttu-id="9cca8-105">Pogledajte [kontrolnu tablu zdrave usluge](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) da biste videli da li je vaša organizacija uticala na njih.</span><span class="sxs-lookup"><span data-stu-id="9cca8-105">Check the [Service health dashboard](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>
  
- <span data-ttu-id="9cca8-106">Korisnici mogu primati *503 server* imate grešku prilikom pokušaja da se krećete na SharePoint ili OneDrive lokacije.</span><span class="sxs-lookup"><span data-stu-id="9cca8-106">Users may receive a *503 server is busy* error when attempting to navigate to SharePoint or OneDrive sites.</span></span> <span data-ttu-id="9cca8-107">Ova greška može biti izazvana pritiskom na SharePoint usluzi.</span><span class="sxs-lookup"><span data-stu-id="9cca8-107">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="9cca8-108">SharePoint Online koristi ograničavanje da bi održao optimalne performanse i pouzdanost usluge SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="9cca8-108">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="9cca8-109">Ograničavanje ograničava broj korisničkih radnji ili istovremenih poziva (po skripti ili kodu) kako bi se sprečilo prekomerno korišćenje resursa.</span><span class="sxs-lookup"><span data-stu-id="9cca8-109">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> <span data-ttu-id="9cca8-110">Više informacija o [ograničavanju pogledajte u sistemu SharePoint online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)</span><span class="sxs-lookup"><span data-stu-id="9cca8-110">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

- <span data-ttu-id="9cca8-111">Ako doživite spore performanse sa **klasičnom** ili **modernom** SharePoint lokacijom ili stranicama, koristite alatku za [dijagnostiku stranice](https://aka.ms/perftool) da biste analizirali stranice.</span><span class="sxs-lookup"><span data-stu-id="9cca8-111">If you experience slow performance with a **classic** or **modern** SharePoint site or page, utilize the [Page Diagnostic tool](https://aka.ms/perftool) to analyze the pages.</span></span>
  
- <span data-ttu-id="9cca8-112">Ako i dalje nailazite na opšte spore performanse, pregledajte resurse na dnu ovog članka: [Uvod u podešavanje performansi za SharePoint online](https://go.microsoft.com/fwlink/?linkid=2024334)</span><span class="sxs-lookup"><span data-stu-id="9cca8-112">If you still experience general slow performance, please review the resources at the bottom of this article: [Introduction to performance tuning for SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334)</span></span>
  