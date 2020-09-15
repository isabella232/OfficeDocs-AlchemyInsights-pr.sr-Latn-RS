---
title: Predvorje
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
- "2673"
- "9000740"
ms.openlocfilehash: 44a930355f1faf8ad747885b72753aaeeb80a6f0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47684964"
---
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a><span data-ttu-id="7a323-102">Kontrolisanje postavki lobija i nivoa učešća u timovima</span><span class="sxs-lookup"><span data-stu-id="7a323-102">Control lobby settings and level of participation in Teams</span></span>

<span data-ttu-id="7a323-103">Ako želite da omogućite svima, uključujući uključivanje, spoljne i anonimne korisnike da biste **zaobišli predvorje**, koristite PowerShell da biste izvršili ovaj zadatak.</span><span class="sxs-lookup"><span data-stu-id="7a323-103">If you'd like to allow everyone, including Dial-in, external, and anonymous users, to **bypass the lobby**, use PowerShell to accomplish this task.</span></span> <span data-ttu-id="7a323-104">Evo primera menjanja smernica globalnog sastanka za vašu organizaciju.</span><span class="sxs-lookup"><span data-stu-id="7a323-104">Here's an example of modifying the global meeting policy for your organization.</span></span>

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

<span data-ttu-id="7a323-105">Ovaj cmdlet trenutno zahteva upotrebu programskog dodatka Skype za posao PowerShell.</span><span class="sxs-lookup"><span data-stu-id="7a323-105">This cmdlet currently requires the use of Skype for Business PowerShell module.</span></span> <span data-ttu-id="7a323-106">Da biste se podesili da koristite ovu cmdlet komandu, pogledajte [Upravljanje smernicama putem PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span><span class="sxs-lookup"><span data-stu-id="7a323-106">To get set up to use this cmdlet, check out [Managing policies via PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).</span></span>

<span data-ttu-id="7a323-107">Kada podesite smernice, morate da je primenjujete na korisnike; ili, ako ste izmenili globalnu smernicu, ona će se automatski primeniti na korisnike.</span><span class="sxs-lookup"><span data-stu-id="7a323-107">Once you’ve set up a policy, you need to apply it to users; or, if you modified the Global policy, it will automatically apply to users.</span></span> <span data-ttu-id="7a323-108">Za promene smernica morate da sačekate najmanje **četiri sata do 24 časa** da bi smernice stupile na snagu.</span><span class="sxs-lookup"><span data-stu-id="7a323-108">For any policy change, you need to wait at least **4 hours up to 24 hours** for the policies to take effect.</span></span> 

<span data-ttu-id="7a323-109">Obavezno Pregledajte dokumentaciju ispod pre nego što načinite ove promene da biste razumeli šta to tačno omogućava.</span><span class="sxs-lookup"><span data-stu-id="7a323-109">Be sure to review the documentation below before making these changes to understand exactly what this allows.</span></span>


## <a name="understanding-teams-meeting-lobby-policy-controls"></a><span data-ttu-id="7a323-110">Razumevanje kontrola tima za sastanke timova</span><span class="sxs-lookup"><span data-stu-id="7a323-110">Understanding Teams meeting lobby policy controls</span></span>

<span data-ttu-id="7a323-111">Ove postavke kontrolišu učesnike sastanka koji čekaju u predvorju pre nego što se prime na sastanak i stepen učešća koji su dozvoljeni na sastanku.</span><span class="sxs-lookup"><span data-stu-id="7a323-111">These settings control which meeting participants wait in the lobby before they are admitted to the meeting and the level of participation they are allowed in a meeting.</span></span> <span data-ttu-id="7a323-112">PowerShell možete koristiti da biste ažurirali postavke smernica za sastanak koje još nisu primenjene (označene "uskoro") u centru administracije timova.</span><span class="sxs-lookup"><span data-stu-id="7a323-112">You can use PowerShell to update meeting policy settings that haven't yet been implemented (labeled "coming soon") in the Teams admin center.</span></span> <span data-ttu-id="7a323-113">Pogledajte ispod za primer PowerShell cmdlet sistema koji omogućava svim korisnicima da zaobilaze predvorje.</span><span class="sxs-lookup"><span data-stu-id="7a323-113">See below for an example PowerShell cmdlet that allows all users to bypass the lobby.</span></span>

- <span data-ttu-id="7a323-114">[Automatski Priznaj](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) da su ljudi po-organizatorske politike koje kontrolišu da li se ljudi direktno pridruže sastanku ili čekaju u predvorju dok ih ne priznaje ovlašćeni korisnik.</span><span class="sxs-lookup"><span data-stu-id="7a323-114">[Automatically admit people](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) is a per-organizer policy that controls whether people join a meeting directly or wait in the lobby until they are admitted by an authenticated user.</span></span>

- <span data-ttu-id="7a323-115">[Omogući anonimnim osobama da započnu sastanak](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) je politika po-Organizer koja kontroliše da li anonimni korisnici, uključujući B2B i federovane korisnike, mogu da se pridruže sastanku korisnika bez ovlašćenog korisnika iz organizacije koja je prisustvovala.</span><span class="sxs-lookup"><span data-stu-id="7a323-115">[Allow anonymous people to start a meeting](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) is a per-organizer policy that controls whether anonymous people, including B2B and federated users, can join the user's meeting without an authenticated user from the organization in attendance.</span></span>

- <span data-ttu-id="7a323-116">[Omogućavanje pozivanjem korisnika da zaobiđe predvorje](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**uskoro**) je politika po-Organizer koja kontroliše da li osobe koje se uključe putem telefona direktno pridruže sastanku ili čekaju u predvorju bez obzira na postavku **automatski Priznaj** .</span><span class="sxs-lookup"><span data-stu-id="7a323-116">[Allow dial-in users to bypass the lobby](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**coming soon**) is a per-organizer policy that controls whether people who dial in by phone join the meeting directly or wait in the lobby regardless of the **Automatically admit people** setting.</span></span>

- <span data-ttu-id="7a323-117">[Dozvolite organizatorima da zamene postavke za predvorje](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**uskoro**) je smernica po-Organizer koje kontrolišu da li organizator sastanka može da zameni postavke predvorja koje je administrator postavio **automatski da prizna ljudima** i **Omogući biranjem pozivalaca da zaobilaze predvorje** kada planiraju novi sastanak.</span><span class="sxs-lookup"><span data-stu-id="7a323-117">[Allow organizers to override lobby settings](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**coming soon**) is a per-organizer policy that controls whether the meeting organizer can override the lobby settings that an admin set in **Automatically admit people** and **Allow dial-in users to bypass the lobby** when they schedule a new meeting.</span></span>

<span data-ttu-id="7a323-118">**Napomena:** Pročitajte [Uređivanje smernica za sastanke u timovima](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) za potpun pregled Microsoft smernica za sastanke.</span><span class="sxs-lookup"><span data-stu-id="7a323-118">**Note:** Read [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) for a complete overview of Microsoft Teams meeting policies.</span></span>
