---
title: Postavke smernica sastanka
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
- "9000734"
- "2657"
ms.openlocfilehash: 39151d3a56cc09a8ae2dd77fb7bf1e99066cc77a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/15/2021
ms.locfileid: "51825457"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a><span data-ttu-id="b0a6f-102">Upravljanje smernicama za sastanke u aplikaciji Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="b0a6f-102">Manage meeting policies in Microsoft Teams</span></span>

<span data-ttu-id="b0a6f-103">**Napomi: Može potrajati i do 24 časa da promene smernica stupi na snagu za korisnike.**</span><span class="sxs-lookup"><span data-stu-id="b0a6f-103">**Note: It can take up to 24 hours for policy changes to take effect for users.**</span></span> <span data-ttu-id="b0a6f-104">Možda nećete moći odmah da menjate nove smernice; sačekajte 4 časa i ponovo pokušajte da izmenite novo kreirane smernice.</span><span class="sxs-lookup"><span data-stu-id="b0a6f-104">You might not be able to make changes to newly created policies immediately; wait 4 hours and attempt to modify a newly created policy again.</span></span>

<span data-ttu-id="b0a6f-105">Smernice za sastanke se koriste za kontrolisanje funkcija koje su dostupne učesnicima sastanka za sastanke koje planiraju korisnici u vašoj organizaciji.</span><span class="sxs-lookup"><span data-stu-id="b0a6f-105">Meeting policies are used to control the features that are available to meeting participants for meetings that are scheduled by users in your organization.</span></span> <span data-ttu-id="b0a6f-106">Neke funkcije smernica za sastanke možda još uvek nisu primenjene u Teams centru aktivnosti (one su označene kao "uskoro" u dokumentaciji).</span><span class="sxs-lookup"><span data-stu-id="b0a6f-106">Some features of meeting policies might not be implemented in the Teams admin center yet (these are labeled "coming soon" in the documentation).</span></span> <span data-ttu-id="b0a6f-107">U ovom slučaju ili ako dobijate grešku kao što je "Trenutno ne možemo da ažuriramo smernice, ali da ih pokušamo ponovo kasnije" u Microsoft Teams centru aktivnosti, preporučujemo da koristite PowerShell za kreiranje ili izmenu smernica za Teams sastanke.</span><span class="sxs-lookup"><span data-stu-id="b0a6f-107">In this case, or if you are getting an error like "We can't update the policy right now but try it again later" in the Microsoft Teams admin center, we recommend that you use PowerShell to create or modify Teams meeting policies.</span></span> 

<span data-ttu-id="b0a6f-108">Dodatne informacije o smernicama za sastanke potražite u sledećim resursima:</span><span class="sxs-lookup"><span data-stu-id="b0a6f-108">For more information about meeting policies, see the following resources:</span></span>

- <span data-ttu-id="b0a6f-109">Da biste saznali više o kreiranju smernica, promenama i dodeljivanju korisnika smernicama, pogledajte upravljanje smernicama za [sastanke u teams.](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams)</span><span class="sxs-lookup"><span data-stu-id="b0a6f-109">To learn about creating policies, making changes, and assigning users to the policy, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span></span>

- <span data-ttu-id="b0a6f-110">Da biste promenili smernice pomoću PowerShell cmdlet cmdlet, pogledajte [Teams Pregled programa PowerShell.](https://docs.microsoft.com/microsoftteams/teams-powershell-overview)</span><span class="sxs-lookup"><span data-stu-id="b0a6f-110">To make policy changes using PowerShell cmdlets, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span> 
    - <span data-ttu-id="b0a6f-111">Morate da koristite [PowerShell modul Skype za posao](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) za smernice za sastanke u programu Teams.</span><span class="sxs-lookup"><span data-stu-id="b0a6f-111">You need to use the [Skype for Business PowerShell module](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) for Teams meeting policies.</span></span> 
    - <span data-ttu-id="b0a6f-112">Pregledajte [\*-CsTeamsMeetingPolicy cmdlets dokumentaciju za](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) više informacija.</span><span class="sxs-lookup"><span data-stu-id="b0a6f-112">Review the [\*-CsTeamsMeetingPolicy cmdlets documentation](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) for more information.</span></span>

