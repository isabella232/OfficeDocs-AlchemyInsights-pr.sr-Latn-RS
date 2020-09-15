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
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a>Kontrolisanje postavki lobija i nivoa učešća u timovima

Ako želite da omogućite svima, uključujući uključivanje, spoljne i anonimne korisnike da biste **zaobišli predvorje**, koristite PowerShell da biste izvršili ovaj zadatak. Evo primera menjanja smernica globalnog sastanka za vašu organizaciju.

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

Ovaj cmdlet trenutno zahteva upotrebu programskog dodatka Skype za posao PowerShell. Da biste se podesili da koristite ovu cmdlet komandu, pogledajte [Upravljanje smernicama putem PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell).

Kada podesite smernice, morate da je primenjujete na korisnike; ili, ako ste izmenili globalnu smernicu, ona će se automatski primeniti na korisnike. Za promene smernica morate da sačekate najmanje **četiri sata do 24 časa** da bi smernice stupile na snagu. 

Obavezno Pregledajte dokumentaciju ispod pre nego što načinite ove promene da biste razumeli šta to tačno omogućava.


## <a name="understanding-teams-meeting-lobby-policy-controls"></a>Razumevanje kontrola tima za sastanke timova

Ove postavke kontrolišu učesnike sastanka koji čekaju u predvorju pre nego što se prime na sastanak i stepen učešća koji su dozvoljeni na sastanku. PowerShell možete koristiti da biste ažurirali postavke smernica za sastanak koje još nisu primenjene (označene "uskoro") u centru administracije timova. Pogledajte ispod za primer PowerShell cmdlet sistema koji omogućava svim korisnicima da zaobilaze predvorje.

- [Automatski Priznaj](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) da su ljudi po-organizatorske politike koje kontrolišu da li se ljudi direktno pridruže sastanku ili čekaju u predvorju dok ih ne priznaje ovlašćeni korisnik.

- [Omogući anonimnim osobama da započnu sastanak](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) je politika po-Organizer koja kontroliše da li anonimni korisnici, uključujući B2B i federovane korisnike, mogu da se pridruže sastanku korisnika bez ovlašćenog korisnika iz organizacije koja je prisustvovala.

- [Omogućavanje pozivanjem korisnika da zaobiđe predvorje](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) (**uskoro**) je politika po-Organizer koja kontroliše da li osobe koje se uključe putem telefona direktno pridruže sastanku ili čekaju u predvorju bez obzira na postavku **automatski Priznaj** .

- [Dozvolite organizatorima da zamene postavke za predvorje](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) (**uskoro**) je smernica po-Organizer koje kontrolišu da li organizator sastanka može da zameni postavke predvorja koje je administrator postavio **automatski da prizna ljudima** i **Omogući biranjem pozivalaca da zaobilaze predvorje** kada planiraju novi sastanak.

**Napomena:** Pročitajte [Uređivanje smernica za sastanke u timovima](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) za potpun pregled Microsoft smernica za sastanke.
