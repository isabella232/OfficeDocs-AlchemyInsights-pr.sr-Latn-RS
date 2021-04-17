---
title: Popravka Microsoft 365 aplikacija Nije moguće pronaći povezane licence za Office
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
- "3421"
- "9001426"
ms.openlocfilehash: 1d717fce77de2f55dfc983d42b7f8d46a8c212e7
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816502"
---
# <a name="fixing-the-microsoft-365-apps-couldnt-find-office-licenses-associated-message"></a><span data-ttu-id="edfdf-102">Popravljanje poruke "Nije moguće pronaći office licence povezane" za Microsoft 365 aplikacije</span><span class="sxs-lookup"><span data-stu-id="edfdf-102">Fixing the Microsoft 365 apps "Couldn't find office licenses associated" message</span></span>

<span data-ttu-id="edfdf-103">Ako primite ovu poruku, pokušajte sledeće:</span><span class="sxs-lookup"><span data-stu-id="edfdf-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="edfdf-104">Proverite postavke zaštitnog zida, antivirusnog softvera i proxy servera da biste potvrdili da ne blokiraju pristup internetu Microsoft 365 aplikacijama.</span><span class="sxs-lookup"><span data-stu-id="edfdf-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="edfdf-105">Pogledajte [članak Microsoft 365 opsezi UL adresa i IP adresa.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span><span class="sxs-lookup"><span data-stu-id="edfdf-105">See [Microsoft 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>
2. <span data-ttu-id="edfdf-106">Uklonite [i ponovo dodignite Office licencu za korisnika](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) na koje ovo utiče.</span><span class="sxs-lookup"><span data-stu-id="edfdf-106">Remove and [reassign the Office license](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) for the affected user.</span></span> 
3. <span data-ttu-id="edfdf-107">Otvorite Office aplikaciju i [odjavite](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) se sa postojećih korisničkih naloga.</span><span class="sxs-lookup"><span data-stu-id="edfdf-107">Open an Office app and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span>
4. <span data-ttu-id="edfdf-108">Idite na postavke operativnog > **Naloge** e-pošte & naloge i uklonite sve radne naloge osim naloga na koje  >  to utiče.</span><span class="sxs-lookup"><span data-stu-id="edfdf-108">Go to Windows Settings > **Accounts** > **Email & accounts**, and remove all work accounts except the affected account.</span></span>
5. <span data-ttu-id="edfdf-109">Idite na postavke operativnog sistema Windows > Pristup poslovnim ili školskim nalozima i prekinite vezu sa svim poslovnim nalozima osim naloga na  >  koji to utiče.</span><span class="sxs-lookup"><span data-stu-id="edfdf-109">Go to Windows Settings > **Accounts** > **Access work or school**, and disconnect all work accounts except the affected account.</span></span>
6. <span data-ttu-id="edfdf-110">Uspostavite početne vrednosti stanja aktivacije sistema Office.</span><span class="sxs-lookup"><span data-stu-id="edfdf-110">Reset the Office activation state.</span></span> <span data-ttu-id="edfdf-111">[Saznajte kako.](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state)</span><span class="sxs-lookup"><span data-stu-id="edfdf-111">[Learn how](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span></span>
7. <span data-ttu-id="edfdf-112">[Prijavite se](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) pomoću korisničkog naloga na koji ovo utiče.</span><span class="sxs-lookup"><span data-stu-id="edfdf-112">[Sign in](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>

<span data-ttu-id="edfdf-113">Dodatna rešenja za rešavanje problema možete da pronađete u odeljku Greške sa nelicenciranim proizvodom i [aktivaciju u programu Office.](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)</span><span class="sxs-lookup"><span data-stu-id="edfdf-113">For additional troubleshooting solutions, see [Unlicensed Product and activation errors in Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>