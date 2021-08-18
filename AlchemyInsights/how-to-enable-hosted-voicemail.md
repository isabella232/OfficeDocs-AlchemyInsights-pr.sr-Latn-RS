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
ms.openlocfilehash: 4042e042554f78febff2073fde6f14db72a6d4e0
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/13/2021
ms.locfileid: "58318662"
---
# <a name="how-to-enable-hosted-voicemail"></a>Kako da omogućite Hosted Voicemail

Da biste omogućili govornu **pošti, HostedVoicemail** mora biti postavljen na $true.

Svojstvo **HostedVoicemail** za korisnika koje koristi udaljeni PowerShell (RPS).

Više informacija o povezivanju sa RPS-om potražite u [Microsoft Teams PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) pregled za više informacija o povezivanju sa RPS-om.

1. The Teams Admin should be logged into Remote PowerShell for Teams.
1. Iz tabele PowerShell odziv Teams da li Teams da pokrene **set-csuser user@contoso.com -HostedVoiceMail $true** gde je sip uri korisnika koji je u pitanju.

**Napomi:** Replicira se promene u smernicama do 24 časa.