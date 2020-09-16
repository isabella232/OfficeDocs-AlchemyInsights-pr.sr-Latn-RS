---
title: Popravka Microsoft 365 aplikacija Žao nam je, imamo poruku o privremenim serverima
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3420"
- "9001430"
ms.openlocfilehash: e00504d318efdea4968ddf98b3ce9591f8993e38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47758259"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a><span data-ttu-id="47c5a-102">Popravka Microsoft 365 aplikacija "Žao nam je, imamo trenutne probleme sa serverom"</span><span class="sxs-lookup"><span data-stu-id="47c5a-102">Fixing the Microsoft 365 apps "Sorry, we are having temporary server issues" message</span></span>

<span data-ttu-id="47c5a-103">Ako primite ovu poruku, Isprobajte sledeće:</span><span class="sxs-lookup"><span data-stu-id="47c5a-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="47c5a-104">Proverite zaštitni zid, antivirusni softver i postavke proxy servera da biste potvrdili da ne blokiraju Internet pristup aplikacijama Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="47c5a-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="47c5a-105">Pogledajte [opseg URL adresa i IP adresa](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="47c5a-105">See [URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="47c5a-106">Idite na **Start**  >  **Run**, a zatim otkucajte **Services. msc**.</span><span class="sxs-lookup"><span data-stu-id="47c5a-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="47c5a-107">Proverite da li su pokrenute sledeće usluge:</span><span class="sxs-lookup"><span data-stu-id="47c5a-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="47c5a-108">Automatsko podešavanje mrežnih uređaja koji su povezani sa mrežom</span><span class="sxs-lookup"><span data-stu-id="47c5a-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="47c5a-109">Usluga liste na mreži</span><span class="sxs-lookup"><span data-stu-id="47c5a-109">Network List Service</span></span>
    - <span data-ttu-id="47c5a-110">Svest o mrežnoj lokaciji</span><span class="sxs-lookup"><span data-stu-id="47c5a-110">Network Location Awareness</span></span>
    - <span data-ttu-id="47c5a-111">Windows evidencija događaja</span><span class="sxs-lookup"><span data-stu-id="47c5a-111">Windows Event Log</span></span>

<span data-ttu-id="47c5a-112">Ako jedna od ovih usluga nije pokrenuta, pokušajte da je pokrenete.</span><span class="sxs-lookup"><span data-stu-id="47c5a-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="47c5a-113">Ako vam je problem da pokrenete uslugu, pokrenete sledeću komandu tako što ćete otvoriti komandnu liniju sa punim dozvolama:</span><span class="sxs-lookup"><span data-stu-id="47c5a-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="47c5a-114">**Sfc/scannow**</span><span class="sxs-lookup"><span data-stu-id="47c5a-114">**sfc /scannow**</span></span>

<span data-ttu-id="47c5a-115">Kada se komanda završi, ponovo pokrenite računar.</span><span class="sxs-lookup"><span data-stu-id="47c5a-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="47c5a-116">Detaljne informacije potražite u članku ["Žao nam je, ne možemo da se poveћemo sa vašim nalogom. Pokušajte ponovo kasnije "Greška prilikom aktiviranja](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="47c5a-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>