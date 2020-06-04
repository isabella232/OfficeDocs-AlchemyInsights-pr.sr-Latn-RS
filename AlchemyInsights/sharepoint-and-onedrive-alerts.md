---
title: Kašnjenja u dobijanju upozorenja na SharePoint i OneDrive
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "2642"
ms.openlocfilehash: 7f1033cec3abec782d1eee3b32128c4c60778913
ms.sourcegitcommit: 8e093114cd31141664e267a7c7b779398d5fdfa8
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 06/04/2020
ms.locfileid: "44563524"
---
# <a name="delays-in-receiving-sharepoint-and-onedrive-alerts"></a><span data-ttu-id="9599f-102">Kašnjenja u dobijanju upozorenja na SharePoint i OneDrive</span><span class="sxs-lookup"><span data-stu-id="9599f-102">Delays in receiving SharePoint and OneDrive alerts</span></span>

- <span data-ttu-id="9599f-103">Prvo proverite fasciklu "Neželjena pošta" ili "bezvredna pošta" u e-poruci.</span><span class="sxs-lookup"><span data-stu-id="9599f-103">First check the Junk or Spam folder in your email.</span></span>
- <span data-ttu-id="9599f-104">Ako **su sva obaveštenja iz više datoteka ili biblioteka odložena**, posetite [kontrolnu tablu za uslugu](https://portal.office.com/adminportal/home?ref=/servicehealth) da biste proverili da li postoje neki savetnici/incidenti koji se mogu imati sa SharePoint ili Exchange serverom.</span><span class="sxs-lookup"><span data-stu-id="9599f-104">If **all alerts from multiple files or libraries are delayed**, visit the [Service Health dashboard](https://portal.office.com/adminportal/home?ref=/servicehealth) to check for any advisories/incidents that may be occurring with SharePoint or Exchange.</span></span> <span data-ttu-id="9599f-105">Moguće je da je to problem sa mogućnošću SharePoint upozorenja ili kašnjenja u e-porukama putem Exchange servera.</span><span class="sxs-lookup"><span data-stu-id="9599f-105">The issue might be with the SharePoint alert capability or delays in emails through Exchange.</span></span> <span data-ttu-id="9599f-106">Takođe obratite pažnju na to da li se isporučuje druga e-pošta – ako to nije moguće, problem će verovatno imati kašnjenja u razmeni.</span><span class="sxs-lookup"><span data-stu-id="9599f-106">Also note whether other email is being delivered—if not, the issue is likely with Exchange delays.</span></span>
- <span data-ttu-id="9599f-107">Ako **pojedinačna uzbuna iz određene datoteke ili biblioteke nije isporučena**, pokušajte da je izbrišete i ponovo kreirate.</span><span class="sxs-lookup"><span data-stu-id="9599f-107">If **an individual alert from a specific file or library is not delivered**, attempt to delete and recreate it.</span></span> <span data-ttu-id="9599f-108">Pogledajte odeljak [Upravljanje, prikazivanje ili brisanje SharePoint obaveštenja](https://support.microsoft.com/office/99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) da biste ponovo kreirali obaveštenje.</span><span class="sxs-lookup"><span data-stu-id="9599f-108">See [Manage, view, or delete SharePoint alerts](https://support.microsoft.com/office/99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) to recreate the alert.</span></span>

> [!NOTE]
> - <span data-ttu-id="9599f-109">Nije moguće poslati obaveštenja grupi distribucije.</span><span class="sxs-lookup"><span data-stu-id="9599f-109">Alerts cannot be sent to a Distribution Group.</span></span> <span data-ttu-id="9599f-110">Podržane su samo bezbednosne i O365 grupe.</span><span class="sxs-lookup"><span data-stu-id="9599f-110">Only Security and O365 groups are supported.</span></span>
> - <span data-ttu-id="9599f-111">Ne možete da prilagodite predloške e-pošte obaveštenja.</span><span class="sxs-lookup"><span data-stu-id="9599f-111">You cannot customize alert email templates.</span></span> <span data-ttu-id="9599f-112">Morate da koristite Microsoft flow ili tok posla SharePoint Designer da biste ih ostvarili.</span><span class="sxs-lookup"><span data-stu-id="9599f-112">You must use Microsoft Flow or SharePoint Designer Workflow to achieve those.</span></span>
