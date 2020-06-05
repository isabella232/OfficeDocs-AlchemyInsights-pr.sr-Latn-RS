---
title: Problemi sa prijavljivanjem u Microsoft 365 aplikacije
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2560"
ms.openlocfilehash: e4f2fea5c2f368ae240614ee1f7bc729338dd75d
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 06/05/2020
ms.locfileid: "44579951"
---
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a><span data-ttu-id="cf16b-102">Popravljanje aplikacija za Microsoft 365 "Nažalost, drugi nalog iz vaše organizacije je već potpisan u poruci</span><span class="sxs-lookup"><span data-stu-id="cf16b-102">Fixing the Microsoft 365 apps "Sorry, another account from your organization is already signed in" message</span></span>

<span data-ttu-id="cf16b-103">Da biste ispravili ovu grešku, pokušajte sledeće:</span><span class="sxs-lookup"><span data-stu-id="cf16b-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="cf16b-104">Uklonite sve poslovne naloge, izuzev sa pogođenim nalogom, koristeći Windows postavke > **pristup poslu ili školi**.</span><span class="sxs-lookup"><span data-stu-id="cf16b-104">Remove all work accounts, except the affected account, using Windows Settings > **Access work or school**.</span></span>
- <span data-ttu-id="cf16b-105">[Obrišite Office akreditive](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) koristeći Windows upravljač akreditivima.</span><span class="sxs-lookup"><span data-stu-id="cf16b-105">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="cf16b-106">**Napomena:** Putanje registratora za Office 2016 su promenjene u 16,0.</span><span class="sxs-lookup"><span data-stu-id="cf16b-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="cf16b-107">(Ex: \Software\microsoft\office\16.0\zajed\identitet\)</span><span class="sxs-lookup"><span data-stu-id="cf16b-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="cf16b-108">Otvorite Office aplikaciju, odaberite stavku **File**"  >  **nalog**za datoteku"  >  **Sign Out**. Zatim se prijavite koristeći korisnički nalog sa važećom licencom.</span><span class="sxs-lookup"><span data-stu-id="cf16b-108">Open an Office app, choose **File** > **Account** > **Sign Out**. Then sign in using a user account with a valid license.</span></span> <span data-ttu-id="cf16b-109">Detaljne informacije potražite u članku [Nalozi u sistemu Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span><span class="sxs-lookup"><span data-stu-id="cf16b-109">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="cf16b-110">Za Mac računar pročitajte članak [Nije moguće prijaviti se u Office 2016 za Mac aplikaciju](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span><span class="sxs-lookup"><span data-stu-id="cf16b-110">For Mac, see [Can't sign in to an Office 2016 for Mac app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span></span>

<span data-ttu-id="cf16b-111">Za više informacija pogledajte odeljak ["Nažalost, drugi nalog iz vaše organizacije je već prijavljen na ovom računaru" u sistemu Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in).</span><span class="sxs-lookup"><span data-stu-id="cf16b-111">For more information, see ["Sorry, another account from your organization is already signed in on this computer" in Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in).</span></span>