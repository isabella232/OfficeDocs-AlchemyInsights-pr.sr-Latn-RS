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
# <a name="how-to-enable-hosted-voicemail"></a><span data-ttu-id="eff1e-102">Kako da omogućite Hostovanu govornu poštu</span><span class="sxs-lookup"><span data-stu-id="eff1e-102">How to enable Hosted Voicemail</span></span>

<span data-ttu-id="eff1e-103">Da biste omogućili govornu poštu, **HostedVoicemail** mora biti podešeno na $TRUE.</span><span class="sxs-lookup"><span data-stu-id="eff1e-103">To enable Voicemail, **HostedVoicemail** must be set to $true.</span></span>

<span data-ttu-id="eff1e-104">**HostedVoicemail** vrednost na korisniku pomoću daljinskog PowerShell (RPS).</span><span class="sxs-lookup"><span data-stu-id="eff1e-104">The **HostedVoicemail** property on the user using Remote PowerShell (RPS).</span></span>

<span data-ttu-id="eff1e-105">Više informacija o povezivanju sa RPS-ima potražite u članku [Prikaz PowerShell Microsoft tima](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) za više informacija o povezivanju sa RPS-ima.</span><span class="sxs-lookup"><span data-stu-id="eff1e-105">For more information on connecting to RPS, see [Microsoft Teams PowerShell Overview](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) for more information on connecting to RPS.</span></span>

1. <span data-ttu-id="eff1e-106">Administrator tima treba da bude prijavljen na daljinsku aplikaciju za timove.</span><span class="sxs-lookup"><span data-stu-id="eff1e-106">The Teams Admin should be logged into Remote PowerShell for Teams.</span></span>
1. <span data-ttu-id="eff1e-107">Iz PowerShell upita administrator tima može da pokreće **setu-csuser User@contoso.com-HostedVoiceMail $TRUE** gde je gutljaj Uri od korisnika u pitanju.</span><span class="sxs-lookup"><span data-stu-id="eff1e-107">From PowerShell prompt the Teams Admin can run **set-csuser user@contoso.com -HostedVoiceMail $true** where the sip uri is of the user in question.</span></span>

> [!NOTE]
> <span data-ttu-id="eff1e-108">Promene smernica mogu da imaju do 24 časa za replikaciju.</span><span class="sxs-lookup"><span data-stu-id="eff1e-108">Changes to policies can take up to 24 hours to replicate.</span></span>