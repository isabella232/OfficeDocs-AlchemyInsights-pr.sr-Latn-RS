---
title: Popravljanje Microsoft 365 aplikacija Žao nam je, imamo poruke o privremenom serveru
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3420"
- "9001430"
ms.openlocfilehash: 6db04a437de8e50af349b5c690791981ae872f14
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 06/05/2020
ms.locfileid: "44582717"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a><span data-ttu-id="c18a5-102">Popravljanje aplikacija za Microsoft 365 "Nažalost, imamo poruku o privremenim problemima na serveru"</span><span class="sxs-lookup"><span data-stu-id="c18a5-102">Fixing the Microsoft 365 apps "Sorry, we are having temporary server issues" message</span></span>

<span data-ttu-id="c18a5-103">Ako dobijete ovu poruku, pokušajte sledeće:</span><span class="sxs-lookup"><span data-stu-id="c18a5-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="c18a5-104">Proverite zaštitni zid, antivirusni softver i proxy postavke da biste potvrdili da ne blokiraju pristup internetu u Microsoft 365 aplikacijama.</span><span class="sxs-lookup"><span data-stu-id="c18a5-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="c18a5-105">Pogledajte [URL adrese i OPSEGE IP adresa](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="c18a5-105">See [URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="c18a5-106">Idite na **početni ekran**  >  **Run**i otkucajte **usluge. msc**.</span><span class="sxs-lookup"><span data-stu-id="c18a5-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="c18a5-107">Uverite se da su sve pokrenute sledeće usluge:</span><span class="sxs-lookup"><span data-stu-id="c18a5-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="c18a5-108">Automatsko podešavanje uređaja povezanih sa mrežom</span><span class="sxs-lookup"><span data-stu-id="c18a5-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="c18a5-109">Usluga liste mreža</span><span class="sxs-lookup"><span data-stu-id="c18a5-109">Network List Service</span></span>
    - <span data-ttu-id="c18a5-110">Svest o mrežnoj lokaciji</span><span class="sxs-lookup"><span data-stu-id="c18a5-110">Network Location Awareness</span></span>
    - <span data-ttu-id="c18a5-111">Windows evidencija događaja</span><span class="sxs-lookup"><span data-stu-id="c18a5-111">Windows Event Log</span></span>

<span data-ttu-id="c18a5-112">Ako neka od ovih usluga nije pokrenuta, pokušajte da ga pokrenete.</span><span class="sxs-lookup"><span data-stu-id="c18a5-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="c18a5-113">Ako imate problem sa pokretanjem usluge, pokrenite sledeću komandu tako što ćete otvoriti komandnu liniju sa punim dozvolama:</span><span class="sxs-lookup"><span data-stu-id="c18a5-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="c18a5-114">**Sfc/scannow**</span><span class="sxs-lookup"><span data-stu-id="c18a5-114">**sfc /scannow**</span></span>

<span data-ttu-id="c18a5-115">Nakon završetka ove komande, ponovo pokrenite računar.</span><span class="sxs-lookup"><span data-stu-id="c18a5-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="c18a5-116">Detaljnije informacije potražite u članku ["Nažalost, ne možemo da se povežemo sa vašim nalogom. Pokušajte ponovo kasnije "Greška prilikom aktiviranja](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="c18a5-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>