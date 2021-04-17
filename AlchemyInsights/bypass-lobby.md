---
title: Zaobilaženje hola
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
- "2673"
- "9000740"
ms.openlocfilehash: bcb40c6f15e957c0a59911322c3b28f03cd562c1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820048"
---
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a><span data-ttu-id="bfa21-102">Kontrolisanje postavki hola i nivo učešća u teams</span><span class="sxs-lookup"><span data-stu-id="bfa21-102">Control lobby settings and level of participation in Teams</span></span>

<span data-ttu-id="bfa21-103">Ako želite da omogućite svima, uključujući uključivanje biranjem, spoljne i anonimne korisnike, da zaobiđu hol pomoću usluge PowerShell da bi izvršili ovaj zadatak.</span><span class="sxs-lookup"><span data-stu-id="bfa21-103">If you'd like to allow everyone, including Dial-in, external, and anonymous users, to **bypass the lobby**, use PowerShell to accomplish this task.</span></span> <span data-ttu-id="bfa21-104">Evo primera izmene globalnih smernica za sastanke za vašu organizaciju.</span><span class="sxs-lookup"><span data-stu-id="bfa21-104">Here's an example of modifying the global meeting policy for your organization.</span></span>

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

<span data-ttu-id="bfa21-105">Ova cmdlet komanda trenutno zahteva korišćenje Modula Skype za posao PowerShell.</span><span class="sxs-lookup"><span data-stu-id="bfa21-105">This cmdlet currently requires the use of Skype for Business PowerShell module.</span></span> <span data-ttu-id="bfa21-106">Da biste se podesili da koristite ovu cmdlet datoteku, pogledajte upravljanje [smernicama putem funkcije PowerShell.](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell)</span><span class="sxs-lookup"><span data-stu-id="bfa21-106">To get set up to use this cmdlet, check out [Managing policies via PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span></span>

<span data-ttu-id="bfa21-107">Kada podesite smernice, morate da ih primenite na korisnike; ili, ako ste izmenili globalne smernice, ona će se automatski primeniti na korisnike.</span><span class="sxs-lookup"><span data-stu-id="bfa21-107">Once you’ve set up a policy, you need to apply it to users; or, if you modified the Global policy, it will automatically apply to users.</span></span> <span data-ttu-id="bfa21-108">Da bi se promenile smernice, morate da čekate najmanje **4 časa do 24 časa** da bi smernice stupile na snagu.</span><span class="sxs-lookup"><span data-stu-id="bfa21-108">For any policy change, you need to wait at least **4 hours up to 24 hours** for the policies to take effect.</span></span> 

<span data-ttu-id="bfa21-109">Uverite se da ste pregledali dokumentaciju u nastavku pre nego što napravite ove promene da biste tačno razumeli šta to dozvoljava.</span><span class="sxs-lookup"><span data-stu-id="bfa21-109">Be sure to review the documentation below before making these changes to understand exactly what this allows.</span></span>


## <a name="understanding-teams-meeting-lobby-policy-controls"></a><span data-ttu-id="bfa21-110">Razumevanje kontrola smernica za sastanke u teams sastanku</span><span class="sxs-lookup"><span data-stu-id="bfa21-110">Understanding Teams meeting lobby policy controls</span></span>

<span data-ttu-id="bfa21-111">Ove postavke kontrolišu koji učesnici na sastanku čekaju u čekaonici pre nego što se prihvate sastanku, kao i nivo učešća koje im je dozvoljeno na sastanku.</span><span class="sxs-lookup"><span data-stu-id="bfa21-111">These settings control which meeting participants wait in the lobby before they are admitted to the meeting and the level of participation they are allowed in a meeting.</span></span> <span data-ttu-id="bfa21-112">Možete da koristite PowerShell da biste ažurirali postavke smernica sastanka koje još nisu primenjene (obeležene kao "uskoro") u Teams centru za administracije.</span><span class="sxs-lookup"><span data-stu-id="bfa21-112">You can use PowerShell to update meeting policy settings that haven't yet been implemented (labeled "coming soon") in the Teams admin center.</span></span> <span data-ttu-id="bfa21-113">U nastavku pogledajte primer PowerShell cmdlet koji svim korisnicima omogućava da zaobiću hol.</span><span class="sxs-lookup"><span data-stu-id="bfa21-113">See below for an example PowerShell cmdlet that allows all users to bypass the lobby.</span></span>

- <span data-ttu-id="bfa21-114">[Automatski prihvataj osobe](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) jesu smernice po organizatoru koje kontrolišu da li se osobe pridružuju sastanku direktno ili čekaju u čekaonici dok ih ovlašćeni korisnik ne primi.</span><span class="sxs-lookup"><span data-stu-id="bfa21-114">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="bfa21-115">[](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) Dozvoli anonimnim osobama da započnu sastanak je smernica po organizatoru koja kontroliše da li anonimne osobe, uključujući B2B i spoljne korisnike, mogu da se pridruže sastanku korisnika bez ovlašćenog korisnika iz organizacije u prisustvu.</span><span class="sxs-lookup"><span data-stu-id="bfa21-115">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="bfa21-116">[Dozvolite](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) korisnicima koji se uključe biranjem da zaobiđu hol **(** uskoro ) su smernice po organizatoru koje kontrolišu  da li se osobe koje pozivaju telefonom direktno pridružuju sastanku ili čekaju u čekaonici bez obzira na postavku Automatski prihvataj osobe.</span><span class="sxs-lookup"><span data-stu-id="bfa21-116">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="bfa21-117">Dozvoli organizatorima da zamene postavke hola **(uskoro**) su [smernice](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) po organizatoru koje kontrolišu da li organizator  sastanka može  da promeni postavke hola koje je postavio administraator u e-pošti Automatski prihvata osobe i Dozvoli korisnicima biranja da zaobiđi hol kada zakazuju novi sastanak.</span><span class="sxs-lookup"><span data-stu-id="bfa21-117">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="bfa21-118">**Napomogućeno:** Pročitajte [članak Upravljanje smernicama za sastanke u aplikaciji Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) da biste dobili potpuni pregled smernica za Microsoft Teams sastanke.</span><span class="sxs-lookup"><span data-stu-id="bfa21-118">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span>
