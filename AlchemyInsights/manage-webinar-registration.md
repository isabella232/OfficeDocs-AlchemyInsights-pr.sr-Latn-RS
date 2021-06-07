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
# <a name="manage-webinar-registration"></a>Upravljanje registracijom vebernara

Vi upravljate ko može da se registruje za Teams vebinare pomoću Teams PowerShell komandama. Da biste instalirali Teams PowerShell, [pogledajte Teams PowerShell](/microsoftteams/teams-powershell-install). 

Prema podrazumevanim *postavkama, whoCanRegister* je omogućen i postavljen na **EveryoneInCompany**. Da biste svima, uključujući anonimne korisnike, dozvolili da se registruju, morate da podesite smernice za sastanke na **Svi** tako što ćete koristiti PowerShell komandu:

`Set-CsTeamsMeetingPolicy -WhoCanRegister Everyone`

**Najava:** Ako je anonimno pridruživanje isključeno u postavkama sastanka, anonimni korisnici ne mogu da se pridruže vebinarima. Da biste saznali više i omogućili ovu postavku, pogledajte [upravljanje postavkama sastanka u Microsoft Teams.](/microsoftteams/meeting-settings-in-teams)

Ako želite da isključite registraciju za sastanak, *postavite vrednost AllowMeetingRegistration na* **Netačno.**

Da biste saznali više o konfigurisanju ko može da se registruje za vebinar, pogledajte konfigurisanje ko može da se [registruje za vebinare.](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars) Dodatne informacije o postavkama za Microsoft liste potražite u [članku Postavke kontrole za Microsoft liste.](/sharepoint/control-lists)
