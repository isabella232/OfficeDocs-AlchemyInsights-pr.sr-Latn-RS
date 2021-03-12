---
title: Postavke smernica sastanka
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
- "9000734"
- "2657"
ms.openlocfilehash: 24a55417df0f89063fbdd9ade6d104be4f8ab49c
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/10/2021
ms.locfileid: "50704620"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a><span data-ttu-id="3bee6-102">Upravljanje smernicama za sastanke u Microsoft timovima</span><span class="sxs-lookup"><span data-stu-id="3bee6-102">Manage meeting policies in Microsoft Teams</span></span>

<span data-ttu-id="3bee6-103">**Napomena: može da potraje do 24 časa da bi promene smernica stupile na snagu za korisnike.**</span><span class="sxs-lookup"><span data-stu-id="3bee6-103">**Note: It can take up to 24 hours for policy changes to take effect for users.**</span></span> <span data-ttu-id="3bee6-104">Možda trenutno ne možete da unesete promene u novokreirane smernice; Sačekajte četiri sata i pokušajte ponovo da izmenite nove kreirane smernice.</span><span class="sxs-lookup"><span data-stu-id="3bee6-104">You might not be able to make changes to newly created policies immediately; wait 4 hours and attempt to modify a newly created policy again.</span></span>

<span data-ttu-id="3bee6-105">Smernice sastanka se koriste za kontrolisanje funkcija koje su dostupne učesnicima sastanka za sastanke koje su zakazali korisnici u vašoj organizaciji.</span><span class="sxs-lookup"><span data-stu-id="3bee6-105">Meeting policies are used to control the features that are available to meeting participants for meetings that are scheduled by users in your organization.</span></span> <span data-ttu-id="3bee6-106">Neke funkcije smernica za sastanak možda se još uvek ne primenjuju u centru administracije timova (ove su označene kao "uskoro" u dokumentaciji).</span><span class="sxs-lookup"><span data-stu-id="3bee6-106">Some features of meeting policies might not be implemented in the Teams admin center yet (these are labeled "coming soon" in the documentation).</span></span> <span data-ttu-id="3bee6-107">U ovom slučaju, ili ako dobijate grešku kao što je "trenutno ne možemo da ažuriramo smernice, ali pokušajte ponovo kasnije" u Microsoft centru administracije, preporučujemo da koristite PowerShell da biste kreirali ili izmenili smernice timova za sastanak.</span><span class="sxs-lookup"><span data-stu-id="3bee6-107">In this case, or if you are getting an error like "We can't update the policy right now but try it again later" in the Microsoft Teams admin center, we recommend that you use PowerShell to create or modify Teams meeting policies.</span></span> 

<span data-ttu-id="3bee6-108">Više informacija o smernicama za sastanak potražite u sledećim resursima:</span><span class="sxs-lookup"><span data-stu-id="3bee6-108">For more information about meeting policies, see the following resources:</span></span>

- <span data-ttu-id="3bee6-109">Da biste saznali više o kreiranju smernica, kreiranju promena i dodeljivanju korisnika smernicama, pogledajte članak [Upravljanje smernicama za sastanke u timovima](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span><span class="sxs-lookup"><span data-stu-id="3bee6-109">To learn about creating policies, making changes, and assigning users to the policy, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).</span></span>

- <span data-ttu-id="3bee6-110">Da biste izmenili promene smernica pomoću PowerShell cmdlet zapisa, pogledajte članak [Power](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span><span class="sxs-lookup"><span data-stu-id="3bee6-110">To make policy changes using PowerShell cmdlets, see [Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview).</span></span> 
    - <span data-ttu-id="3bee6-111">Treba da koristite aplikaciju [Skype za posao PowerShell](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) za smernice za sastanke timova.</span><span class="sxs-lookup"><span data-stu-id="3bee6-111">You need to use the [Skype for Business PowerShell module](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) for Teams meeting policies.</span></span> 
    - <span data-ttu-id="3bee6-112">Pregledajte više informacija [\*-c, smietingpolicy cmdlet dokumentaciju](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) .</span><span class="sxs-lookup"><span data-stu-id="3bee6-112">Review the [\*-CsTeamsMeetingPolicy cmdlets documentation](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) for more information.</span></span>

