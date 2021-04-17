---
title: Popravljanje Microsoft 365 aplikacija Žao nam je, imamo poruku o privremenim problemima sa serverom
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3420"
- "9001430"
ms.openlocfilehash: 0adf1d66869051b9dd8290ef3466ef9b13aa2d41
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/15/2021
ms.locfileid: "51835285"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a><span data-ttu-id="4ea21-102">Rešavanje poruke "Žao nam je, imamo privremene probleme sa serverom" za Microsoft 365 aplikacije</span><span class="sxs-lookup"><span data-stu-id="4ea21-102">Fixing the Microsoft 365 apps "Sorry, we are having temporary server issues" message</span></span>

<span data-ttu-id="4ea21-103">Ako primite ovu poruku, pokušajte sledeće:</span><span class="sxs-lookup"><span data-stu-id="4ea21-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="4ea21-104">Proverite postavke zaštitnog zida, antivirusnog softvera i proxy servera da biste potvrdili da ne blokiraju pristup internetu Microsoft 365 aplikacijama.</span><span class="sxs-lookup"><span data-stu-id="4ea21-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="4ea21-105">Pogledajte [UL adrese i opsege IP adresa](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="4ea21-105">See [URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="4ea21-106">Idite na **Start**  >  **Run**, a zatim **otkucajte services.msc**.</span><span class="sxs-lookup"><span data-stu-id="4ea21-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="4ea21-107">Uverite se da su sve sledeće usluge pokrenute:</span><span class="sxs-lookup"><span data-stu-id="4ea21-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="4ea21-108">Automatsko podešavanje uređaja koji su povezani sa mrežom</span><span class="sxs-lookup"><span data-stu-id="4ea21-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="4ea21-109">Usluga "Lista mreža"</span><span class="sxs-lookup"><span data-stu-id="4ea21-109">Network List Service</span></span>
    - <span data-ttu-id="4ea21-110">Svest o mrežnoj lokaciji</span><span class="sxs-lookup"><span data-stu-id="4ea21-110">Network Location Awareness</span></span>
    - <span data-ttu-id="4ea21-111">Windows evidencija događaja</span><span class="sxs-lookup"><span data-stu-id="4ea21-111">Windows Event Log</span></span>

<span data-ttu-id="4ea21-112">Ako jedna od ovih usluga nije pokrenuta, pokušajte da je pokrenete.</span><span class="sxs-lookup"><span data-stu-id="4ea21-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="4ea21-113">Ako imate problema sa pokretanjem usluge, pokrenite sledeću komandu tako što ćete otvoriti komandnu liniju sa punim dozvolama:</span><span class="sxs-lookup"><span data-stu-id="4ea21-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="4ea21-114">**sfc /scannow**</span><span class="sxs-lookup"><span data-stu-id="4ea21-114">**sfc /scannow**</span></span>

<span data-ttu-id="4ea21-115">Kada se ova komanda završi, ponovo pokrenite računar.</span><span class="sxs-lookup"><span data-stu-id="4ea21-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="4ea21-116">Detaljne informacije potražite u [temi "Žao nam je, ne možemo da se povežemo sa vašim nalogom. Greška "Pokušajte ponovo kasnije" prilikom aktiviranja.](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)</span><span class="sxs-lookup"><span data-stu-id="4ea21-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>