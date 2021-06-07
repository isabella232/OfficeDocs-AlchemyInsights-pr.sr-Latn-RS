---
title: Upravljanje registracijom vebernara
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/02/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11512"
- "9006672"
ms.openlocfilehash: c5b0721d286b07d7e0f84199885b6f527a2b42a2
ms.sourcegitcommit: f7a9e97d04b7b6cbb633b32094d40f1874bf0fce
ms.translationtype: HT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 06/06/2021
ms.locfileid: "52794147"
---
# <a name="manage-webinar-registration"></a><span data-ttu-id="ede56-102">Upravljanje registracijom vebernara</span><span class="sxs-lookup"><span data-stu-id="ede56-102">Manage webinar registration</span></span>

<span data-ttu-id="ede56-103">Vi upravljate ko može da se registruje za Teams vebinare pomoću Teams PowerShell komandama.</span><span class="sxs-lookup"><span data-stu-id="ede56-103">You manage who can register for Teams Webinars by using Teams Powershell commands.</span></span> <span data-ttu-id="ede56-104">Da biste instalirali Teams PowerShell, [pogledajte Teams PowerShell](/microsoftteams/teams-powershell-install).</span><span class="sxs-lookup"><span data-stu-id="ede56-104">To install Teams Powershell, see [Teams PowerShell](/microsoftteams/teams-powershell-install).</span></span> 

<span data-ttu-id="ede56-105">Prema podrazumevanim *postavkama, whoCanRegister* je omogućen i postavljen na **EveryoneInCompany**.</span><span class="sxs-lookup"><span data-stu-id="ede56-105">By default, *WhoCanRegister* is enabled and set to **EveryoneInCompany**.</span></span> <span data-ttu-id="ede56-106">Da biste svima, uključujući anonimne korisnike, dozvolili da se registruju, morate da podesite smernice za sastanke na **Svi** tako što ćete koristiti PowerShell komandu:</span><span class="sxs-lookup"><span data-stu-id="ede56-106">To allow anyone, including anonymous users, to register, you must set the Meeting Policy to **Everyone** by using the Powershell command:</span></span>

`Set-CsTeamsMeetingPolicy -WhoCanRegister Everyone`

<span data-ttu-id="ede56-107">**Najava:** Ako je anonimno pridruživanje isključeno u postavkama sastanka, anonimni korisnici ne mogu da se pridruže vebinarima.</span><span class="sxs-lookup"><span data-stu-id="ede56-107">**Note**: If anonymous join is turned off in meeting settings, anonymous users can't join webinars.</span></span> <span data-ttu-id="ede56-108">Da biste saznali više i omogućili ovu postavku, pogledajte [upravljanje postavkama sastanka u Microsoft Teams.](/microsoftteams/meeting-settings-in-teams)</span><span class="sxs-lookup"><span data-stu-id="ede56-108">To learn more and enable this setting, see [Manage meeting settings in Microsoft Teams](/microsoftteams/meeting-settings-in-teams).</span></span>

<span data-ttu-id="ede56-109">Ako želite da isključite registraciju za sastanak, *postavite vrednost AllowMeetingRegistration na* **Netačno.**</span><span class="sxs-lookup"><span data-stu-id="ede56-109">If you want to turn off meeting registration, set *AllowMeetingRegistration* to **False**.</span></span>

<span data-ttu-id="ede56-110">Da biste saznali više o konfigurisanju ko može da se registruje za vebinar, pogledajte konfigurisanje ko može da se [registruje za vebinare.](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars)</span><span class="sxs-lookup"><span data-stu-id="ede56-110">To learn more about configuring who can register for webinars, see [Configure who can register for webinars](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars).</span></span> <span data-ttu-id="ede56-111">Dodatne informacije o postavkama za Microsoft liste potražite u [članku Postavke kontrole za Microsoft liste.](/sharepoint/control-lists)</span><span class="sxs-lookup"><span data-stu-id="ede56-111">For more information about settings for Microsoft Lists, see [Control settings for Microsoft Lists](/sharepoint/control-lists).</span></span>
