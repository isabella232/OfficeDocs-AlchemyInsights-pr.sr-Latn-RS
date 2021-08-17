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
ms.openlocfilehash: dac6690b66181455a1c9c0f40a642b71f2af3516d91ea0853d06564b017b03a2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "54059610"
---
# <a name="control-lobby-settings-and-level-of-participation-in-teams"></a>Kontrolisanje postavki hola i nivo učešća u Teams

Ako želite da omogućite svima, uključujući uključivanje biranjem, spoljne i anonimne korisnike, da zaobiđu hol pomoću usluge PowerShell da bi izvršili ovaj zadatak. Evo primera izmene globalnih smernica za sastanke za vašu organizaciju.

`Set-CsTeamsMeetingPolicy -Identity Global -AutoAdmittedUsers "Everyone" -AllowPSTNUsersToBypassLobby $True`

Ova cmdlet komanda trenutno zahteva upotrebu Skype za posao PowerShell modulu. Da biste se podesili da koristite ovu cmdlet datoteku, pogledajte upravljanje [smernicama putem funkcije PowerShell.](https://docs.microsoft.com/microsoftteams/teams-powershell-overview#managing-policies-via-powershell)

Kada podesite smernice, morate da ih primenite na korisnike; ili, ako ste izmenili globalne smernice, ona će se automatski primeniti na korisnike. Da bi se promenile smernice, morate da čekate najmanje **4 časa do 24 časa** da bi smernice stupile na snagu. 

Uverite se da ste pregledali dokumentaciju u nastavku pre nego što napravite ove promene da biste tačno razumeli šta to dozvoljava.


## <a name="understanding-teams-meeting-lobby-policy-controls"></a>Razumevanje Teams kontrola smernica za sastanke

Ove postavke kontrolišu koji učesnici na sastanku čekaju u čekaonici pre nego što se prihvate sastanku, kao i nivo učešća koje im je dozvoljeno na sastanku. Možete da koristite PowerShell da biste ažurirali postavke smernica sastanka koje još nisu primenjene (obeležene kao "uskoro") u Teams centru za administracije. U nastavku pogledajte primer PowerShell cmdlet koji svim korisnicima omogućava da zaobiću hol.

- [Automatski prihvataj osobe](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#automatically-admit-people) jesu smernice po organizatoru koje kontrolišu da li se osobe pridružuju sastanku direktno ili čekaju u čekaonici dok ih ovlašćeni korisnik ne primi.

- [](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-anonymous-people-to-start-a-meeting) Dozvoli anonimnim osobama da započnu sastanak je smernica po organizatoru koja kontroliše da li anonimne osobe, uključujući B2B i spoljne korisnike, mogu da se pridruže sastanku korisnika bez ovlašćenog korisnika iz organizacije u prisustvu.

- [Dozvolite](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-dial-in-users-to-bypass-the-lobby-coming-soon) korisnicima koji se uključe biranjem da zaobiđu hol **(** uskoro ) su smernice po organizatoru koje kontrolišu  da li se osobe koje pozivaju telefonom direktno pridružuju sastanku ili čekaju u čekaonici bez obzira na postavku Automatski prihvataj osobe.

- Dozvoli organizatorima da zamene postavke hola **(uskoro**) su [smernice](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-organizers-to-override-lobby-settings-coming-soon) po organizatoru koje kontrolišu da li organizator  sastanka može  da promeni postavke hola koje je postavio administraator u e-pošti Automatski prihvata osobe i Dozvoli korisnicima biranja da zaobiđi hol kada zakazuju novi sastanak.

**Napomogućeno:** Pročitajte [upravljanje smernicama za sastanke Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams) da biste dobili potpuni pregled smernica Microsoft Teams sastanka.
