---
title: Problemi sa prijavljivanjem u Microsoft 365 aplikacije
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
- "9000571"
- "2560"
ms.openlocfilehash: 7d2cfd437bb55804c3b9263428833c10d5caaa47
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695337"
---
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a><span data-ttu-id="db314-102">Popravka Microsoft 365 aplikacija "Žao nam je, drugi nalog iz vaše organizacije je već prijavljen"</span><span class="sxs-lookup"><span data-stu-id="db314-102">Fixing the Microsoft 365 apps "Sorry, another account from your organization is already signed in" message</span></span>

<span data-ttu-id="db314-103">Da biste ispravili ovu grešku, pokušajte sledeće:</span><span class="sxs-lookup"><span data-stu-id="db314-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="db314-104">Uklanjanje svih naloga za posao, osim naloga koji je uticao, pomoću Windows postavki > **Access poslu ili školi**.</span><span class="sxs-lookup"><span data-stu-id="db314-104">Remove all work accounts, except the affected account, using Windows Settings > **Access work or school**.</span></span>
- <span data-ttu-id="db314-105">[Brisanje Office akreditiva](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) pomoću upravljača Windows akreditivima.</span><span class="sxs-lookup"><span data-stu-id="db314-105">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="db314-106">**Napomena:** Putanje registratora za Office 2016 su promenjene u 16,0.</span><span class="sxs-lookup"><span data-stu-id="db314-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="db314-107">(Ex: \Software\microsoft\office\16.0\local \ identitet\)</span><span class="sxs-lookup"><span data-stu-id="db314-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="db314-108">Otvorite Office aplikaciju, odaberite stavku **File**  >  **nalog naloga**za datoteku  >  **Sign Out**. Zatim se prijavite pomoću korisničkog naloga sa važećom licencom.</span><span class="sxs-lookup"><span data-stu-id="db314-108">Open an Office app, choose **File** > **Account** > **Sign Out**. Then sign in using a user account with a valid license.</span></span> <span data-ttu-id="db314-109">Detaljne informacije potražite u članku [Nalozi u sistemu Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span><span class="sxs-lookup"><span data-stu-id="db314-109">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="db314-110">Za Mac računar pročitajte članak [Nije moguće prijaviti se u Office 2016 za Mac aplikaciju](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span><span class="sxs-lookup"><span data-stu-id="db314-110">For Mac, see [Can't sign in to an Office 2016 for Mac app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span></span>

<span data-ttu-id="db314-111">Više informacija potražite u članku ["Žao nam je, drugi nalog iz vaše organizacije je već prijavljen na ovom računaru" u sistemu Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in).</span><span class="sxs-lookup"><span data-stu-id="db314-111">For more information, see ["Sorry, another account from your organization is already signed in on this computer" in Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in).</span></span>