---
title: Nije moguće aktivirati Office
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "2000023"
- "3509"
ms.openlocfilehash: 81941d84127a096c3bd588dafc61b492ab6d6458
ms.sourcegitcommit: 1eee2412dfb8b1f10a3aa28dd1086a0c589cdba0
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 06/07/2021
ms.locfileid: "52798694"
---
# <a name="unable-to-activate-office"></a><span data-ttu-id="713e0-102">Nije moguće aktivirati Office</span><span class="sxs-lookup"><span data-stu-id="713e0-102">Unable to activate Office</span></span>

<span data-ttu-id="713e0-103">Na primer: Ako koristite stariju verziju programa Windows (na primer, Windows 7), **uverite** se da je TLS 1.2 omogućen kao podrazumevani.</span><span class="sxs-lookup"><span data-stu-id="713e0-103">**Note**: If you are using an older version of Windows (For example, Windows 7), ensure that TLS 1.2 is enabled as the default.</span></span> <span data-ttu-id="713e0-104">Više informacija potražite u temi Ažuriranje da biste omogućili [TLS 1.1 i TLS 1.2](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)kao podrazumevane bezbedne protokole u winHTTP-u Windows.</span><span class="sxs-lookup"><span data-stu-id="713e0-104">For more information, see [Update to enable TLS 1.1 and TLS 1.2 as default secure protocols in WinHTTP in Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392).</span></span>

- <span data-ttu-id="713e0-105">Proverite da li je istekao status pretplate.</span><span class="sxs-lookup"><span data-stu-id="713e0-105">Check if your subscription status has expired.</span></span>
- <span data-ttu-id="713e0-106">Proverite da li imate pretplatu koja dozvoljava klijentske licence, kao što su Office 365 Business ili Business Premium, i [proverite da li je korisniku dodeljena licenca](/microsoft-365/admin/manage/assign-licenses-to-users).</span><span class="sxs-lookup"><span data-stu-id="713e0-106">Ensure you have a subscription that allows client licenses, such as Office 365 Business or Business Premium, and [ensure the user has a license assigned](/microsoft-365/admin/manage/assign-licenses-to-users).</span></span>
- <span data-ttu-id="713e0-107">Proverite da li se korisnik prijavljuje u Office sa istim nalogom na kojem ima dodeljenu licencu.</span><span class="sxs-lookup"><span data-stu-id="713e0-107">Ensure the user is signing into Office with the same account that has the license assigned.</span></span>
- <span data-ttu-id="713e0-108">Posetite [stranicu ispravnosti sistema Office 365](/office365/enterprise/view-service-health) da biste videli da li postoje poznati problemi sa uslugom.</span><span class="sxs-lookup"><span data-stu-id="713e0-108">Check the [Office 365 Service Health page](/office365/enterprise/view-service-health) to see if there are any known problems with the service.</span></span>
- <span data-ttu-id="713e0-109">Proverite zaštitni zid, antivirusni program i postavke proxy servera da biste potvrdili da ne blokiraju pristup Microsoft 365 aplikacija internetu.</span><span class="sxs-lookup"><span data-stu-id="713e0-109">Check your firewall, antivirus software and proxy settings to confirm that they are not blocking Microsoft 365 apps access to the internet.</span></span> <span data-ttu-id="713e0-110">Pogledajte članak [Opsezi URL i IP adresa sistema Office 365](/office365/enterprise/urls-and-ip-address-ranges "Opsezi URL i IP adresa sistema Office 365").</span><span class="sxs-lookup"><span data-stu-id="713e0-110">Please see [Office 365 URLs and IP address ranges](/office365/enterprise/urls-and-ip-address-ranges "Office 365 URLs and IP address ranges").</span></span>

<span data-ttu-id="713e0-111">**Savet** Na računarima sa operativnim sistemom Windows, možemo da dijagnostikujemo nekoliko uobičajenih problema sa prijavljivanjem u Office i da ih automatski otklonimo za vas.</span><span class="sxs-lookup"><span data-stu-id="713e0-111">**Tip** On Windows machines, we can diagnose and automatically fix several common Office sign-in issues for you.</span></span> <span data-ttu-id="713e0-112">Preuzmite i pokrenite aplikaciju  **[Microsoft pomoćnik za podršku i oporavak](https://aka.ms/SaRA-OfficeSignInScenario)** da biste koristili našu automatizovanu alatku.</span><span class="sxs-lookup"><span data-stu-id="713e0-112">Download and run the  **[Microsoft Support and Recovery Assistant](https://aka.ms/SaRA-OfficeSignInScenario)** to use our automated tool.</span></span>

<span data-ttu-id="713e0-113">Koristite sledeće radnje za rešavanju problema:</span><span class="sxs-lookup"><span data-stu-id="713e0-113">Use the following troubleshooting actions:</span></span>

- <span data-ttu-id="713e0-114">Otvorite Office aplikaciju i [odjavite se](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) sa bilo kog postojećeg korisničkog naloga.</span><span class="sxs-lookup"><span data-stu-id="713e0-114">Open an Office app, and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span> <span data-ttu-id="713e0-115">[Uklonite](/microsoft-365/admin/manage/remove-licenses-from-users) i [ponovo dodelite](/microsoft-365/admin/manage/assign-licenses-to-users) licencu za Office, a zatim [prijavite se u Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) pomoću korisničkog naloga.</span><span class="sxs-lookup"><span data-stu-id="713e0-115">[Remove](/microsoft-365/admin/manage/remove-licenses-from-users) and [re-assign](/microsoft-365/admin/manage/assign-licenses-to-users) Office license, and then [sign into Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>
- <span data-ttu-id="713e0-116">Pokrenite [Alatku za rešavanje problema sa aktivacijom](https://aka.ms/SARA-OfficeActivation-Alchemy)</span><span class="sxs-lookup"><span data-stu-id="713e0-116">Run the [Activation Troubleshooter](https://aka.ms/SARA-OfficeActivation-Alchemy)</span></span>
- [<span data-ttu-id="713e0-117">Resetovanje stanja aktivacije sistema Office</span><span class="sxs-lookup"><span data-stu-id="713e0-117">Reset Office activation state</span></span>](/office365/troubleshoot/activation/reset-office-365-proplus-activation-state "Uspostavljanje početne vrednosti stanja aktivacije sistema Office")
- [<span data-ttu-id="713e0-118">Obavite popravku na mreži sistema Office</span><span class="sxs-lookup"><span data-stu-id="713e0-118">Perform an Online Repair of Office</span></span>](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b?wt.mc_id=Alchemy_ClientDIA)

<span data-ttu-id="713e0-119">Dodatna rešenja za rešavanje problema potražite u članku:</span><span class="sxs-lookup"><span data-stu-id="713e0-119">For additional troubleshooting solutions, see:</span></span>  

- [<span data-ttu-id="713e0-120">Greška „Nelicencirani proizvod“ i greška aktivacije u sistemu Office</span><span class="sxs-lookup"><span data-stu-id="713e0-120">Unlicensed Product and activation errors in Office</span></span>](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380?wt.mc_id=Alchemy_ClientDIA)
- [<span data-ttu-id="713e0-121">„Žao nam je, ne možemo da se povežemo sa nalogom. Pokušajte ponovo kasnije“ – greška prilikom aktiviranja sistema Office</span><span class="sxs-lookup"><span data-stu-id="713e0-121">"Sorry, we can't connect to your account. Please try again later" error when you activate Office</span></span>](/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)