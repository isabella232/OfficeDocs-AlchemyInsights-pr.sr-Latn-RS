---
title: 1491-rezultati
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1491"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: 5c4452726c1dbe2232ee63e8a9ee4d089f5c76db
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47740488"
---
# <a name="content-search-not-returning-expected-results"></a><span data-ttu-id="50bc5-102">Pretraga sadržaja ne vraća očekivane rezultate</span><span class="sxs-lookup"><span data-stu-id="50bc5-102">Content Search not returning expected results</span></span>

<span data-ttu-id="50bc5-103">Prilikom pokretanja Pretraga sadržaja iz Microsoft 365 Security & centra za usaglašenost, možda ćete dobiti neočekivane rezultate pretrage.</span><span class="sxs-lookup"><span data-stu-id="50bc5-103">When running Content Searches from the Microsoft 365 security & Compliance Center, you may receive unexpected search results.</span></span> <span data-ttu-id="50bc5-104">Razmotrite sledeće stvari koje mogu da utiču na rezultate pretrage:</span><span class="sxs-lookup"><span data-stu-id="50bc5-104">Consider the following things that can affect your search results:</span></span>

- <span data-ttu-id="50bc5-105">**Lokacije sadržaja i uslovi pretrage**: uverite se da ste izabrali odgovarajuće lokacije sadržaja i uslove pretrage.</span><span class="sxs-lookup"><span data-stu-id="50bc5-105">**Content locations and search conditions**: Make sure you have selected the proper content locations and search conditions.</span></span> <span data-ttu-id="50bc5-106">Ako ste pokrenuli veliku pretragu (sa mnogo lokacija), razmotrite da je razdelite u više pretraga.</span><span class="sxs-lookup"><span data-stu-id="50bc5-106">If you ran a large search (with many locations), consider splitting it into multiple searches.</span></span>

- <span data-ttu-id="50bc5-107">**Delimično indeksirane stavke**:  [delimično indeksirane](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) stavke iz poštanskog sandučića obuhvaćene su procenjenim rezultatima pretrage.</span><span class="sxs-lookup"><span data-stu-id="50bc5-107">**Partially indexed items**:  [Partially indexed items](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) from mailboxes are included in the estimated search results.</span></span> <span data-ttu-id="50bc5-108">Međutim, delimično indeksirane stavke sa lokacija u sistemu SharePoint i OneDrive nisu uključene u procenu pretrage.</span><span class="sxs-lookup"><span data-stu-id="50bc5-108">However, partially indexed items from sites in SharePoint and OneDrive aren't included in the search estimate.</span></span>

- <span data-ttu-id="50bc5-109">**Otkazivanja pretrage**: kada pretražujete veliki broj poštanskih sandučića (preko 100.000 poštanskih sandučića), možete da dobijete greške prilikom pretrage sa kodom greške kao što su CS008-009 i CS012-002).</span><span class="sxs-lookup"><span data-stu-id="50bc5-109">**Search failures**: When searching a large number of mailboxes (over 100,000 mailboxes), you may get search errors, with error codes such as CS008-009 and CS012-002).</span></span> <span data-ttu-id="50bc5-110">U ovom slučaju ponovo pokušajte da izvršite pretragu samo za lokacije koje nisu uspele.</span><span class="sxs-lookup"><span data-stu-id="50bc5-110">In this case, retry the search only for the failed content locations.</span></span> <span data-ttu-id="50bc5-111">Više informacija potražite u  [članku ovaj članak](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) .</span><span class="sxs-lookup"><span data-stu-id="50bc5-111">See  [this article](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) for more information.</span></span>
