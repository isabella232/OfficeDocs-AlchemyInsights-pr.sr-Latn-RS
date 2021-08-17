---
title: Kako da omogućite Hosted Voicemail
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/09/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002347"
- "7563"
ms.openlocfilehash: 4d70e92a7c1bf8f3cc62d4a310aa140ee2dfdef4c798ae17faa961736d9db500
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "54055568"
---
# <a name="how-to-enable-hosted-voicemail"></a>Kako da omogućite Hosted Voicemail

Da biste omogućili govornu **pošti, HostedVoicemail** mora biti postavljen na $true.

Svojstvo **HostedVoicemail** za korisnika koje koristi udaljeni PowerShell (RPS).

Više informacija o povezivanju sa RPS-om potražite u [Microsoft Teams PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) pregled za više informacija o povezivanju sa RPS-om.

1. Teams treba da bude prijavljen u udaljeni PowerShell za Teams.
1. Iz tabele PowerShell odziv Teams Da li Teams da pokrene **set-csuser user@contoso.com -HostedVoiceMail $true** gde je sip uri korisnika koji je u pitanju.

> [!NOTE]
> Replicira se promene na smernicama do 24 časa.