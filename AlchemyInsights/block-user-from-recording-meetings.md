---
title: Blokiranje korisnika iz snimanja sastanaka
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002530"
- "9325"
ms.openlocfilehash: 3f633ee1fb3329b6fc634acabbc824af1eccfb33
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037070"
---
# <a name="block-user-from-recording-meetings"></a><span data-ttu-id="eec83-102">Blokiranje korisnika iz snimanja sastanaka</span><span class="sxs-lookup"><span data-stu-id="eec83-102">Block User From Recording Meetings</span></span>

<span data-ttu-id="eec83-103">Ako treba da **sprečite ili blokirate** određenim korisnicima da biste snimili sastanke timova, to možete da uradite pomoću postavki timova za sastanke.</span><span class="sxs-lookup"><span data-stu-id="eec83-103">If you need to **prevent or block** specific users from recording Teams Meetings, you can do so via Teams Meeting Policy settings.</span></span> <span data-ttu-id="eec83-104">U Microsoft centru administracije, isključite postavku " **Omogući snimanje u oblaku** " u smernicama sastanka dodeljene tom korisniku.</span><span class="sxs-lookup"><span data-stu-id="eec83-104">In the Microsoft Teams admin center, turn off the **Allow cloud recording** setting in the meeting policy assigned to that user.</span></span> <span data-ttu-id="eec83-105">Da biste saznali više, pogledajte članak [Upravljanje smernicama za sastanke u timovima](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-cloud-recording).</span><span class="sxs-lookup"><span data-stu-id="eec83-105">To learn more, see [Manage meeting policies in Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams#allow-cloud-recording).</span></span>

<span data-ttu-id="eec83-106">Da biste proverili valjanost ako je određen korisnik dozvoljen ili nije da biste snimali sastanke timova, koristite dijagnostiku podrške.</span><span class="sxs-lookup"><span data-stu-id="eec83-106">To validate if a specific user is allowed or not to record Teams Meetings, use the support diagnostic.</span></span> <span data-ttu-id="eec83-107">Izvršite novi upit za podršku i otkucajte **Diag: snimak sastanka** – dijagnostika će proveravati postavke smernica za navedenog korisnika i odrediti postavke smernica.</span><span class="sxs-lookup"><span data-stu-id="eec83-107">Run a new support query and type in **Diag: Meeting Recording** - the diagnostic will check policy settings for the specified user and determine their policy settings.</span></span> <span data-ttu-id="eec83-108">Upamtite, može da potraje nekoliko sati da bi nove postavke smernica stupile na snagu, tako da ako ste upravo napravili promene, sačekajte nekoliko sati pre nego što ponovo pokrenete dijagnostiku.</span><span class="sxs-lookup"><span data-stu-id="eec83-108">Remember, it can take a couple of hours for new policy settings to take effect, so if you have just made a change, wait a few hours before running the diagnostic again.</span></span>

<span data-ttu-id="eec83-109">Dodatne informacije potražite u redigovanja [Uključivanje ili isključivanje snimanja oblaka](https://docs.microsoft.com/microsoftteams/cloud-recording#turn-on-or-turn-off-cloud-recording).</span><span class="sxs-lookup"><span data-stu-id="eec83-109">For more information, review [Turn on or turn off cloud recording](https://docs.microsoft.com/microsoftteams/cloud-recording#turn-on-or-turn-off-cloud-recording).</span></span>
