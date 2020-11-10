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
# <a name="using-giphys-in-teams-conversations"></a>Korišćenje programa Giphys u razgovorima timova

Giphys pristup u timske ćaskanja podrazumevano je omogućen. Kao administrator, možete kontrolisati da li su korisnici dostupni korisnicima tako što ćete [podesiti smernice za razmenu poruka](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) i osigurati da se **koriste gifrys u razgovorima** . **On**

Ako GIF ne radi na očekivani način u razgovorima timova, potvrdite sledeće:

[Smernica za razmenu poruka](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) mora da omogući Giphys. Da biste proverili pomoću programa PowerShell cmdlet:

- Proverite da li možete da [upravljate timovima sa PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell).
- Pokretanje komande PowerShell za Power for [-c. Smissagingpolicy-identitet Global](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) i Verifikujte da je **Allowgiphy** postavljen na **TRUE**.
- Ako je **Allowgiphy** podešen na **FALSE** , uradite sledeće PowerShell komande [-C, Smissagingpolicy-identitet Global-allowgiphy $TRUE](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps).

[Opcionalna povezana iskustva](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) treba da se omogući da omogućite pristup GIFIJOM URL adresi.

> [!NOTE]
> Ako imate više smernica za razmenu poruka timova koje su podešene za zakupca, možete da utvrdite identitet smernica dodeljenih uticajenim korisnicima pomoću komande Command Power [-CsOnlineUser-identitet](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> | Izaberite stavku Teamsmissagingpolicy.
