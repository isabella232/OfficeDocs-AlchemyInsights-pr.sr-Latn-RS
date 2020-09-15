---
title: Klasiиni izveštaji o SharePoint nadzornoj evidenciji
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: daf79f8d75ccdff8ad54f0f307648a5832a6bb71
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47662222"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a><span data-ttu-id="ce714-102">SharePoint i OneDrive evidencija nadzora</span><span class="sxs-lookup"><span data-stu-id="ce714-102">SharePoint and OneDrive audit logs</span></span>

## <a name="sharepoint-classic-audit-logs"></a><span data-ttu-id="ce714-103">SharePoint Classic evidencija nadzora</span><span class="sxs-lookup"><span data-stu-id="ce714-103">SharePoint classic Audit logs</span></span>

<span data-ttu-id="ce714-104">Zastarelo nadgledanje SPO-a je migriralo u objedinjenu evidenciju nadzora (UAL).</span><span class="sxs-lookup"><span data-stu-id="ce714-104">SPO legacy auditing was migrated to Unified Audit Log (UAL).</span></span> <span data-ttu-id="ce714-105">Svi izveštaji SPO-ve za zastareli nadzor će se sada primeniti na UAL, a signali zastarelog nadzora su migrirali u UAL.</span><span class="sxs-lookup"><span data-stu-id="ce714-105">All SPO legacy audit reports will now be powered through UAL, and the legacy audit signals have been migrated to UAL.</span></span>

<span data-ttu-id="ce714-106">Promene ključnih stavki:</span><span class="sxs-lookup"><span data-stu-id="ce714-106">Key changes:</span></span>

* <span data-ttu-id="ce714-107">Skraćivanje skraćivanja nije dostupno kao mogućnost.</span><span class="sxs-lookup"><span data-stu-id="ce714-107">Trimming is NOT available as a capability.</span></span>
* <span data-ttu-id="ce714-108">Biranje određenih događaja za nadgledanje nije dostupno.</span><span class="sxs-lookup"><span data-stu-id="ce714-108">Choosing specific events to audit is NOT available.</span></span> <span data-ttu-id="ce714-109">Pogledajte [ovaj dokument](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance) za kompletnu listu revizija događaja dostupnih po podrazumevanoj vrednosti.</span><span class="sxs-lookup"><span data-stu-id="ce714-109">Refer to [this document](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance) for a complete list of audited events available by default.</span></span>
* <span data-ttu-id="ce714-110">Opcija **lokacije** u okviru **prilagođeni izveštaji** nije dostupna.</span><span class="sxs-lookup"><span data-stu-id="ce714-110">The **Location** option under **Customized reports** is NOT available.</span></span>
* <span data-ttu-id="ce714-111">Opcija " **Otvaranje" ili "preuzimanje dokumenata** " nije dostupna.</span><span class="sxs-lookup"><span data-stu-id="ce714-111">The **Opening or downloading documents** events option is NOT available.</span></span>

[<span data-ttu-id="ce714-112">Konfigurisanje postavki nadgledanja za kolekciju lokacija</span><span class="sxs-lookup"><span data-stu-id="ce714-112">Configure Audit settings for a site collection</span></span>](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a><span data-ttu-id="ce714-113">SharePoint i OneDrive moderne evidentirate nadzora iz usaglašenosti</span><span class="sxs-lookup"><span data-stu-id="ce714-113">SharePoint and OneDrive Modern Unified Audit logs from compliance</span></span>

* [<span data-ttu-id="ce714-114">Uključivanje/isključivanje objedinjenog evidentiranja nadzora</span><span class="sxs-lookup"><span data-stu-id="ce714-114">Turn on/off Unified Audit Logging</span></span>](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off) 

<span data-ttu-id="ce714-115">U sistemu SharePoint ili OneDrive nije potrebna dodatna konfiguracija.</span><span class="sxs-lookup"><span data-stu-id="ce714-115">No additional configuration is required within SharePoint or OneDrive.</span></span>

<span data-ttu-id="ce714-116">Korišćenje pretrage evidentiranja nadzora radi provere aktivnosti datoteka, fascikli, korisnika, dozvola:</span><span class="sxs-lookup"><span data-stu-id="ce714-116">Use audit logging search to check activity of the file(s), folder(s), user(s), permissions:</span></span>

* [<span data-ttu-id="ce714-117">Aktivnosti datoteka i stranica</span><span class="sxs-lookup"><span data-stu-id="ce714-117">File and page activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance)
* [<span data-ttu-id="ce714-118">Aktivnosti fascikle</span><span class="sxs-lookup"><span data-stu-id="ce714-118">Folder activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [<span data-ttu-id="ce714-119">Aktivnosti deljenja i pristupa</span><span class="sxs-lookup"><span data-stu-id="ce714-119">Sharing and access request activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [<span data-ttu-id="ce714-120">Aktivnosti sinhronizacije</span><span class="sxs-lookup"><span data-stu-id="ce714-120">Synchronization activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [<span data-ttu-id="ce714-121">Aktivnosti administracije sajta</span><span class="sxs-lookup"><span data-stu-id="ce714-121">Site administration activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

<span data-ttu-id="ce714-122">Više informacija o tome kako da preuzmete ove događaje potražite [u članku Pretraga evidencije nadzora](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span><span class="sxs-lookup"><span data-stu-id="ce714-122">For more information about how to retrieve these events, see [Search the audit log](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span>
