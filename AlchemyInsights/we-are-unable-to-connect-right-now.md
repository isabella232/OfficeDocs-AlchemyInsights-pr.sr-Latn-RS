---
title: Problem sa aktivacijom – trenutno ne možemo da se poveћemo
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
- "3408"
- "9001423"
ms.openlocfilehash: 24fe9910d1715b4f5f7d8d06b1d1344d4b8675bc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47725997"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a><span data-ttu-id="822e4-102">Popravka Microsoft 365 aplikacija "trenutno ne možemo da se poveћemo" poruka</span><span class="sxs-lookup"><span data-stu-id="822e4-102">Fixing the Microsoft 365 apps "We are unable to connect right now" message</span></span>

<span data-ttu-id="822e4-103">Ako primite ovu poruku, Isprobajte sledeće:</span><span class="sxs-lookup"><span data-stu-id="822e4-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="822e4-104">Proverite zaštitni zid, antivirusni softver i postavke proxy servera da biste potvrdili da ne blokiraju Internet pristup aplikacijama Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="822e4-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="822e4-105">Pogledajte [opsege Microsoft URL adresa i IP adresa](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="822e4-105">See [Microsoft URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="822e4-106">Idite na **Start**  >  **Run**, a zatim otkucajte **Services. msc**.</span><span class="sxs-lookup"><span data-stu-id="822e4-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="822e4-107">Proverite da li su pokrenute sledeće usluge:</span><span class="sxs-lookup"><span data-stu-id="822e4-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="822e4-108">Automatsko podešavanje mrežnih uređaja koji su povezani sa mrežom</span><span class="sxs-lookup"><span data-stu-id="822e4-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="822e4-109">Usluga liste na mreži</span><span class="sxs-lookup"><span data-stu-id="822e4-109">Network List Service</span></span>
    - <span data-ttu-id="822e4-110">Svest o mrežnoj lokaciji</span><span class="sxs-lookup"><span data-stu-id="822e4-110">Network Location Awareness</span></span>
    - <span data-ttu-id="822e4-111">Windows evidencija događaja</span><span class="sxs-lookup"><span data-stu-id="822e4-111">Windows Event Log</span></span>

<span data-ttu-id="822e4-112">Ako jedna od ovih usluga nije pokrenuta, pokušajte da je pokrenete.</span><span class="sxs-lookup"><span data-stu-id="822e4-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="822e4-113">Ako vam je problem da pokrenete uslugu, pokrenete sledeću komandu tako što ćete otvoriti komandnu liniju sa punim dozvolama:</span><span class="sxs-lookup"><span data-stu-id="822e4-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="822e4-114">**Sfc/scannow**</span><span class="sxs-lookup"><span data-stu-id="822e4-114">**sfc /scannow**</span></span>

<span data-ttu-id="822e4-115">Kada se komanda završi, ponovo pokrenite računar.</span><span class="sxs-lookup"><span data-stu-id="822e4-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="822e4-116">Detaljne informacije potražite u članku ["Žao nam je, ne možemo da se poveћemo sa vašim nalogom. Pokušajte ponovo kasnije "Greška prilikom aktiviranja sistema Office sa Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="822e4-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate Office from Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>