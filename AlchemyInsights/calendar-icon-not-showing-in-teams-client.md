---
title: Ikona kalendara se ne prikazuje u Teams klijentu
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001219"
- "4375"
ms.openlocfilehash: 6a3f02b69d160c7dce68ed03df59c0d7d1f32f0f
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819967"
---
# <a name="calendar-icon-not-showing-in-teams-client"></a><span data-ttu-id="69da1-102">Ikona kalendara se ne prikazuje u Teams klijentu</span><span class="sxs-lookup"><span data-stu-id="69da1-102">Calendar icon not showing in Teams client</span></span>

<span data-ttu-id="69da1-103">Kartica „Kalendar“ u usluzi Teams zahteva pristup Exchange poštanskom sandučetu putem veb usluga programa Exchange.</span><span class="sxs-lookup"><span data-stu-id="69da1-103">The Calendar Tab in Teams requires access to an Exchange mailbox via Exchange Web Services.</span></span> <span data-ttu-id="69da1-104">Exchange poštansko sanduče može da bude na mreži ili lokalno.</span><span class="sxs-lookup"><span data-stu-id="69da1-104">The Exchange mailbox can be Online or On-Premises.</span></span> <span data-ttu-id="69da1-105">Za korisnike na mreži koji ne vide karticu „Kalendar“, uverite se da su [licencirani za Exchange Online poštansko sanduče i da je poštansko sanduče omogućeno](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).</span><span class="sxs-lookup"><span data-stu-id="69da1-105">For Online users who do not see the Calendar Tab, make sure they [are licensed for an Exchange Online mailbox and the mailbox is enabled](https://docs.microsoft.com/exchange/recipients-in-exchange-online/create-user-mailboxes).</span></span>

<span data-ttu-id="69da1-106">Ako korisnik ima važeće poštansko sanduče u usluzi Exchange Online, ali i dalje ne može da vidi karticu „Kalendar“, možda imate problem sa mrežom.</span><span class="sxs-lookup"><span data-stu-id="69da1-106">If the user has a valid mailbox in Exchange Online, but still cannot see the Calendar tab, you may be experiencing a network issue.</span></span> <span data-ttu-id="69da1-107">Koristite [Microsoft analizator daljinske mogućnosti povezivanja](https://testconnectivity.microsoft.com/) i pokrenite **Microsoft Exchange testove mogućnosti povezivanja veb usluga** za korisnika na koga ovo utiče.</span><span class="sxs-lookup"><span data-stu-id="69da1-107">Use the [Microsoft Remote Connectivity Analyzer](https://testconnectivity.microsoft.com/) and run the **Microsoft Exchange Web Services Connectivity Tests** for the impacted user.</span></span>

<span data-ttu-id="69da1-108">Na kraju proverite [Teams aplikacije – smernice za podešavanje aplikacija](https://admin.teams.microsoft.com/policies/app-setup) da biste se uverili da aplikacija Kalendar nije uklonjena iz smernica primenjenih na korisnika (verovatno su u pitanju **Globalne (podrazumevane za celu organizaciju)**.</span><span class="sxs-lookup"><span data-stu-id="69da1-108">Finally check the [Teams Apps – App setup policies](https://admin.teams.microsoft.com/policies/app-setup) to ensure the Calendar app has not been removed from the policy applied to the user (most likely the **Global (Org-wide default)**.</span></span>

<span data-ttu-id="69da1-109">Ako vaši korisnici rade lokalno kod kuće, treba da potvrdite da je vaša hibridna konfiguracija ispravna.</span><span class="sxs-lookup"><span data-stu-id="69da1-109">If your users are homed On-Premises, you need to confirm your Hybrid configuration is healthy.</span></span> <span data-ttu-id="69da1-110">Koristite [Čarobnjak za hibridnu konfiguraciju](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) da biste rešili problem.</span><span class="sxs-lookup"><span data-stu-id="69da1-110">Use the [Hybrid Configuration Wizard](https://docs.microsoft.com/exchange/hybrid-deployment/hybrid-agent) to troubleshoot.</span></span>

<span data-ttu-id="69da1-111">Imajte u vidu da [Teams zahteva Exchange 2016 CU3 ili noviju verziju](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).</span><span class="sxs-lookup"><span data-stu-id="69da1-111">Note that [Teams requires Exchange 2016 CU3 or higher](https://docs.microsoft.com/microsoftteams/exchange-teams-interact).</span></span>
