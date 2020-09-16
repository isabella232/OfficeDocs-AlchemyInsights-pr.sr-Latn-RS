---
title: Popravka Microsoft 365 aplikacija nije mogla da pronađe pridruženu poruku za Office licence
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
- "3421"
- "9001426"
ms.openlocfilehash: bd127d6287b4438f6105a6158abdbd5b964b7e70
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47747709"
---
# <a name="fixing-the-microsoft-365-apps-couldnt-find-office-licenses-associated-message"></a><span data-ttu-id="9938a-102">Ispravljanje Microsoft 365 aplikacija "nije bilo povezano sa porukom Office licenci"</span><span class="sxs-lookup"><span data-stu-id="9938a-102">Fixing the Microsoft 365 apps "Couldn't find office licenses associated" message</span></span>

<span data-ttu-id="9938a-103">Ako primite ovu poruku, Isprobajte sledeće:</span><span class="sxs-lookup"><span data-stu-id="9938a-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="9938a-104">Proverite zaštitni zid, antivirusni softver i postavke proxy servera da biste potvrdili da ne blokiraju Internet pristup aplikacijama Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="9938a-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="9938a-105">Pogledajte [Microsoft 365 URL adrese i OPSEGE IP adresa](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="9938a-105">See [Microsoft 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>
2. <span data-ttu-id="9938a-106">Uklonite i [ponovo dodelite Office licencu](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) za pogođene korisnike.</span><span class="sxs-lookup"><span data-stu-id="9938a-106">Remove and [reassign the Office license](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) for the affected user.</span></span> 
3. <span data-ttu-id="9938a-107">Otvorite Office aplikaciju i [odjavite](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) se sa bilo kog postojećeg korisničkog naloga.</span><span class="sxs-lookup"><span data-stu-id="9938a-107">Open an Office app and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span>
4. <span data-ttu-id="9938a-108">Idite na Windows Settings > **nalozima**  >  **&** nalozima i uklonite sve naloge za posao osim naloga koji je uticao.</span><span class="sxs-lookup"><span data-stu-id="9938a-108">Go to Windows Settings > **Accounts** > **Email & accounts**, and remove all work accounts except the affected account.</span></span>
5. <span data-ttu-id="9938a-109">Idite na postavke operativnog sistema Windows > **nalozima**u operativnom sistemu  >  **Access**i isključite sve naloge za posao osim naloga koji je uticao.</span><span class="sxs-lookup"><span data-stu-id="9938a-109">Go to Windows Settings > **Accounts** > **Access work or school**, and disconnect all work accounts except the affected account.</span></span>
6. <span data-ttu-id="9938a-110">Poništite stanje sistema Office.</span><span class="sxs-lookup"><span data-stu-id="9938a-110">Reset the Office activation state.</span></span> <span data-ttu-id="9938a-111">[Saznajte kako](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span><span class="sxs-lookup"><span data-stu-id="9938a-111">[Learn how](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span></span>
7. <span data-ttu-id="9938a-112">[Prijavite](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) se koristeći korisnik koji utiče na njega.</span><span class="sxs-lookup"><span data-stu-id="9938a-112">[Sign in](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>

<span data-ttu-id="9938a-113">Dodatne rešenja za rešavanje problema potražite [u članku nelicencirane greške proizvoda i aktivacije u sistemu Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span><span class="sxs-lookup"><span data-stu-id="9938a-113">For additional troubleshooting solutions, see [Unlicensed Product and activation errors in Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>