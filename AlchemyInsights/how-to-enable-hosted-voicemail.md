---
title: Kako da omogućite Hostovanu govornu poštu
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
ms.openlocfilehash: 26eb22054d246a6ca5a2491c68a5d9e4ed90d45b
ms.sourcegitcommit: 523098560e54a50184a99c974809dfbfffadacb5
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 12/09/2020
ms.locfileid: "49679167"
---
# <a name="how-to-enable-hosted-voicemail"></a>Kako da omogućite Hostovanu govornu poštu

Da biste omogućili govornu poštu, **HostedVoicemail** mora biti podešeno na $TRUE.

**HostedVoicemail** vrednost na korisniku pomoću daljinskog PowerShell (RPS).

Više informacija o povezivanju sa RPS-ima potražite u članku [Prikaz PowerShell Microsoft tima](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) za više informacija o povezivanju sa RPS-ima.

1. Administrator tima treba da bude prijavljen na daljinsku aplikaciju za timove.
1. Iz PowerShell upita administrator tima može da pokreće **setu-csuser User@contoso.com-HostedVoiceMail $TRUE** gde je gutljaj Uri od korisnika u pitanju.

> [!NOTE]
> Promene smernica mogu da imaju do 24 časa za replikaciju.