---
title: Korišćenje Giphy-a u Teams razgovorima
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
ms.openlocfilehash: 0244b68ffa2ebd3d70bae66a24ac299004848557b63b17c2ea74fafaff22bb8c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "54104322"
---
# <a name="using-giphys-in-teams-conversations"></a>Korišćenje Giphy-a u Teams razgovorima

Giphys pristup u Teams ćaskanja podrazumevano je omogućen. Kao administrator možete da kontrolišete da li su [](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams#messaging-policy-settings) Giphy-je dostupni korisnicima tako što ćete postaviti smernice za razmenu poruka i da se uverite da je postavka Korišćenje **Giphy-ova** u razgovorima bila **"Na"**.

Ako GIF-ove ne rade na očekivani način Teams razgovorima, proverite:

Smernice [za razmenu](https://docs.microsoft.com/microsoftteams/messaging-policies-in-teams) poruka moraju da dozvole giphys. Da biste to verifikuli pomoću PowerShell cmdlet cmdlet mina:

- Uverite se da možete [da upravljate Teams powerShell.](https://docs.microsoft.com/microsoftteams/teams-powershell-overview?view=o365-worldwide#manage-teams-with-powershell)
- Pokrenite PowerShell [komandu Get-CsTeamsMessagingPolicy -Identity Global](https://docs.microsoft.com/powershell/module/skype/get-csteamsmessagingpolicy?view=skype-ps) i potvrdite da je **AllowGiphy** postavljen na **TRUE.**
- Ako **je vrednost AllowGiphy** postavljena na **FALSE,** pokrenite sledeću PowerShell komandu [Set-CsTeamsMessagingPolicy -Identity Global -AllowGiphy $True.](https://docs.microsoft.com/powershell/module/skype/set-csteamsmessagingpolicy?view=skype-ps)

[Opcionalna povezana iskustva](https://docs.microsoft.com/deployoffice/privacy/optional-connected-experiences) moraju biti omogućena da bi se dozvolio pristup Giphy URL adresi.

> [!NOTE]
> Ako imate više smernica Teams za razmenu poruka konfigurisanih za zakupac, možete da utvrdite identitet smernica dodeljenih korisniku na koje ovo utiče sa PowerShell komandom [Get-CsOnlineUser -Identity](https://docs.microsoft.com/powershell/module/skype/get-csonlineuser?view=skype-ps) <user@domain.com> | Izaberite TeamsMessagingPolicy.
