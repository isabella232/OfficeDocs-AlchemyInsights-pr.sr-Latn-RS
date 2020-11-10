---
title: Korišćenje programa Giphys u razgovorima timova
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003825"
- "6850"
ms.openlocfilehash: 2fc29974bff9484c226c9651b9b000a89cad14dc
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 11/09/2020
ms.locfileid: "48982579"
---
# <a name="using-giphys-in-teams-conversations"></a><span data-ttu-id="2e975-102">Korišćenje programa Giphys u razgovorima timova</span><span class="sxs-lookup"><span data-stu-id="2e975-102">Using Giphys in Teams Conversations</span></span>

<span data-ttu-id="2e975-103">Giphys pristup u timske ćaskanja podrazumevano je omogućen.</span><span class="sxs-lookup"><span data-stu-id="2e975-103">Giphys access in Teams chat is enabled by default.</span></span> <span data-ttu-id="2e975-104">Kao administrator, možete kontrolisati da li su korisnici dostupni korisnicima tako što ćete [podesiti smernice za razmenu poruka](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) i osigurati da se **koriste gifrys u razgovorima** . **On**</span><span class="sxs-lookup"><span data-stu-id="2e975-104">As an administrator, you can control if Giphys are available to users by [setting a messaging policy](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) and ensuring that **Use Giphys in conversations** is **On**.</span></span>

<span data-ttu-id="2e975-105">Ako GIF ne radi na očekivani način u razgovorima timova, potvrdite sledeće:</span><span class="sxs-lookup"><span data-stu-id="2e975-105">If GIFs are not working as expected in Teams conversations, verify:</span></span>

<span data-ttu-id="2e975-106">[Smernica za razmenu poruka](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) mora da omogući Giphys.</span><span class="sxs-lookup"><span data-stu-id="2e975-106">The [messaging policy](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) needs to allow Giphys.</span></span> <span data-ttu-id="2e975-107">Da biste proverili pomoću programa PowerShell cmdlet:</span><span class="sxs-lookup"><span data-stu-id="2e975-107">To verify by using PowerShell cmdlets:</span></span>

- <span data-ttu-id="2e975-108">Proverite da li možete da [upravljate timovima sa PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell).</span><span class="sxs-lookup"><span data-stu-id="2e975-108">Verify that you can [Manage Teams with PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell).</span></span>
- <span data-ttu-id="2e975-109">Pokretanje komande PowerShell za Power for [-c. Smissagingpolicy-identitet Global](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) i Verifikujte da je **Allowgiphy** postavljen na **TRUE**.</span><span class="sxs-lookup"><span data-stu-id="2e975-109">Run the PowerShell command [Get-CsTeamsMessagingPolicy -Identity Global](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) and verify that **AllowGiphy** is set to **TRUE**.</span></span>
- <span data-ttu-id="2e975-110">Ako je **Allowgiphy** podešen na **FALSE** , uradite sledeće PowerShell komande [-C, Smissagingpolicy-identitet Global-allowgiphy $TRUE](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps).</span><span class="sxs-lookup"><span data-stu-id="2e975-110">If **AllowGiphy** is set to **FALSE** , run the following PowerShell command [Set-CsTeamsMessagingPolicy -Identity Global -AllowGiphy $True](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps).</span></span>

<span data-ttu-id="2e975-111">[Opcionalna povezana iskustva](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) treba da se omogući da omogućite pristup GIFIJOM URL adresi.</span><span class="sxs-lookup"><span data-stu-id="2e975-111">[Optional Connected Experiences](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) need to be enabled to allow access to the Giphy URL.</span></span>

> [!NOTE]
> <span data-ttu-id="2e975-112">Ako imate više smernica za razmenu poruka timova koje su podešene za zakupca, možete da utvrdite identitet smernica dodeljenih uticajenim korisnicima pomoću komande Command Power [-CsOnlineUser-identitet](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> | Izaberite stavku Teamsmissagingpolicy.</span><span class="sxs-lookup"><span data-stu-id="2e975-112">If you have multiple Teams Messaging policies configured for your tenant, you can determine the identity of the policy assigned to the impacted user with the PowerShell command [Get-CsOnlineUser -Identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> | Select TeamsMessagingPolicy.</span></span>
