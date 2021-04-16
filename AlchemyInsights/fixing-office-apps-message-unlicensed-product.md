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
ms.openlocfilehash: 9771a3244c5507312d43156525095fb9eaf7fa20
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/15/2021
ms.locfileid: "51812586"
---
# <a name="unable-to-activate-office"></a><span data-ttu-id="dd511-102">Nije moguće aktivirati Office</span><span class="sxs-lookup"><span data-stu-id="dd511-102">Unable to activate Office</span></span>

- <span data-ttu-id="dd511-103">Proverite da li je istekao status pretplate.</span><span class="sxs-lookup"><span data-stu-id="dd511-103">Check if your subscription status has expired.</span></span>
- <span data-ttu-id="dd511-104">Proverite da li imate pretplatu koja dozvoljava klijentske licence, kao što su Office 365 Business ili Business Premium, i [proverite da li je korisniku dodeljena licenca](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="dd511-104">Ensure you have a subscription that allows client licenses, such as Office 365 Business or Business Premium, and [ensure the user has a license assigned](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users?view=o365-worldwide).</span></span>
- <span data-ttu-id="dd511-105">Proverite da li se korisnik prijavljuje u Office sa istim nalogom na kojem ima dodeljenu licencu.</span><span class="sxs-lookup"><span data-stu-id="dd511-105">Ensure the user is signing into Office with the same account that has the license assigned.</span></span>
- <span data-ttu-id="dd511-106">Posetite [stranicu ispravnosti sistema Office 365](https://docs.microsoft.com/office365/enterprise/view-service-health) da biste videli da li postoje poznati problemi sa uslugom.</span><span class="sxs-lookup"><span data-stu-id="dd511-106">Check the [Office 365 Service Health page](https://docs.microsoft.com/office365/enterprise/view-service-health) to see if there are any known problems with the service.</span></span>
- <span data-ttu-id="dd511-107">Proverite zaštitni zid, antivirusni program i postavke proxy servera da biste potvrdili da ne blokiraju pristup Microsoft 365 aplikacija internetu.</span><span class="sxs-lookup"><span data-stu-id="dd511-107">Check your firewall, antivirus software and proxy settings to confirm that they are not blocking Microsoft 365 apps access to the internet.</span></span> <span data-ttu-id="dd511-108">Pogledajte članak [Opsezi URL i IP adresa sistema Office 365](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges "Opsezi URL i IP adresa sistema Office 365").</span><span class="sxs-lookup"><span data-stu-id="dd511-108">Please see [Office 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges "Office 365 URLs and IP address ranges").</span></span>

<span data-ttu-id="dd511-109">**Savet** Na računarima sa operativnim sistemom Windows, možemo da dijagnostikujemo nekoliko uobičajenih problema sa prijavljivanjem u Office i da ih automatski otklonimo za vas.</span><span class="sxs-lookup"><span data-stu-id="dd511-109">**Tip** On Windows machines, we can diagnose and automatically fix several common Office sign-in issues for you.</span></span> <span data-ttu-id="dd511-110">Preuzmite i pokrenite aplikaciju  **[Microsoft pomoćnik za podršku i oporavak](https://aka.ms/SaRA-OfficeSignInScenario)** da biste koristili našu automatizovanu alatku.</span><span class="sxs-lookup"><span data-stu-id="dd511-110">Download and run the  **[Microsoft Support and Recovery Assistant](https://aka.ms/SaRA-OfficeSignInScenario)** to use our automated tool.</span></span>

<span data-ttu-id="dd511-111">Koristite sledeće radnje za rešavanju problema:</span><span class="sxs-lookup"><span data-stu-id="dd511-111">Use the following troubleshooting actions:</span></span>

- <span data-ttu-id="dd511-112">Otvorite Office aplikaciju i [odjavite se](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) sa bilo kog postojećeg korisničkog naloga.</span><span class="sxs-lookup"><span data-stu-id="dd511-112">Open an Office app, and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span> <span data-ttu-id="dd511-113">[Uklonite](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) i [ponovo dodelite](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) licencu za Office, a zatim [prijavite se u Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) pomoću korisničkog naloga.</span><span class="sxs-lookup"><span data-stu-id="dd511-113">[Remove](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) and [re-assign](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) Office license, and then [sign into Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>
- <span data-ttu-id="dd511-114">Pokrenite [Alatku za rešavanje problema sa aktivacijom](https://aka.ms/SARA-OfficeActivation-Alchemy)</span><span class="sxs-lookup"><span data-stu-id="dd511-114">Run the [Activation Troubleshooter](https://aka.ms/SARA-OfficeActivation-Alchemy)</span></span>
- [<span data-ttu-id="dd511-115">Resetovanje stanja aktivacije sistema Office</span><span class="sxs-lookup"><span data-stu-id="dd511-115">Reset Office activation state</span></span>](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state "Uspostavljanje početne vrednosti stanja aktivacije sistema Office")
- [<span data-ttu-id="dd511-116">Obavite popravku na mreži sistema Office</span><span class="sxs-lookup"><span data-stu-id="dd511-116">Perform an Online Repair of Office</span></span>](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b?wt.mc_id=Alchemy_ClientDIA)

<span data-ttu-id="dd511-117">Dodatna rešenja za rešavanje problema potražite u članku:</span><span class="sxs-lookup"><span data-stu-id="dd511-117">For additional troubleshooting solutions, see:</span></span>  

- [<span data-ttu-id="dd511-118">Greška „Nelicencirani proizvod“ i greška aktivacije u sistemu Office</span><span class="sxs-lookup"><span data-stu-id="dd511-118">Unlicensed Product and activation errors in Office</span></span>](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380?wt.mc_id=Alchemy_ClientDIA)
- [<span data-ttu-id="dd511-119">„Žao nam je, ne možemo da se povežemo sa nalogom. Pokušajte ponovo kasnije“ – greška prilikom aktiviranja sistema Office</span><span class="sxs-lookup"><span data-stu-id="dd511-119">"Sorry, we can't connect to your account. Please try again later" error when you activate Office</span></span>](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)