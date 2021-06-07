---
title: Omogućavanje Teams veinara
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
- "11513"
- "9006672"
ms.openlocfilehash: 5a732e6746e9fd23e54a0b2ffeabb59623012a0e
ms.sourcegitcommit: 9de78b30602f917d58705057cdcce31fec349969
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 06/04/2021
ms.locfileid: "52793780"
---
# <a name="enable-teams-webinars"></a><span data-ttu-id="4bef7-102">Omogućavanje Teams veinara</span><span class="sxs-lookup"><span data-stu-id="4bef7-102">Enable Teams Webinars</span></span>

<span data-ttu-id="4bef7-103">Velineri su podrazumevano omogućeni.</span><span class="sxs-lookup"><span data-stu-id="4bef7-103">Webinars are enabled by default.</span></span> <span data-ttu-id="4bef7-104">Možete da upravljate ko može da planira i registruje termine za Teams tako što ćete koristiti Teams PowerShell komande.</span><span class="sxs-lookup"><span data-stu-id="4bef7-104">You can manage who can schedule and register for Teams Webinars by using Teams PowerShell commands.</span></span>

- <span data-ttu-id="4bef7-105">Svi korisnici koji mogu da kreiraju sastanak takođe mogu da kreiraju sastanak u veb pregledaču.</span><span class="sxs-lookup"><span data-stu-id="4bef7-105">All users who can create a meeting can also create a webinar meeting.</span></span> <span data-ttu-id="4bef7-106">Ako želite da upravljate ko može da planira Teams na vebinarima, *koristite AllowMeetingRegistration*.</span><span class="sxs-lookup"><span data-stu-id="4bef7-106">If you want to manage who can schedule Teams Webinars, use *AllowMeetingRegistration*.</span></span> 
- <span data-ttu-id="4bef7-107">Prema podrazumevanim *postavkama, opcija WhoCanRegister* je omogućena i postavljena na **Svi.**</span><span class="sxs-lookup"><span data-stu-id="4bef7-107">By default, *WhoCanRegister* is enabled and set to **Everyone**.</span></span> <span data-ttu-id="4bef7-108">Ako želite da isključite registraciju za sastanak, *postavite vrednost AllowMeetingRegistration na* **Netačno.**</span><span class="sxs-lookup"><span data-stu-id="4bef7-108">If you want to turn off meeting registration, set *AllowMeetingRegistration* to **False**.</span></span>

<span data-ttu-id="4bef7-109">Da biste promenili ove postavke, morate da [instalirate Teams PowerShell](/microsoftteams/teams-powershell-install).</span><span class="sxs-lookup"><span data-stu-id="4bef7-109">To change these settings, you must install [Teams PowerShell](/microsoftteams/teams-powershell-install).</span></span> <span data-ttu-id="4bef7-110">Takođe, smernice za sastanke primenjene su na Teams velinera.</span><span class="sxs-lookup"><span data-stu-id="4bef7-110">Also, Meeting Policies are enforced on Teams Webinars.</span></span> <span data-ttu-id="4bef7-111">Na primer, ako je anonimno pridruživanje isključeno u postavkama sastanka, anonimni korisnici ne mogu da se pridruže vebinarima.</span><span class="sxs-lookup"><span data-stu-id="4bef7-111">For example, if anonymous join is turned off in meeting settings, anonymous users can't join webinars.</span></span>

<span data-ttu-id="4bef7-112">Da biste saznali više o konfigurisanju ko može da se registruje za vebinar, pogledajte konfigurisanje ko može da se [registruje za vebinare.](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars)</span><span class="sxs-lookup"><span data-stu-id="4bef7-112">To learn more about configuring who can register for webinars, see [Configure who can register for webinars](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars).</span></span> <span data-ttu-id="4bef7-113">Dodatne informacije o postavkama za Microsoft liste potražite u [članku Postavke kontrole za Microsoft liste.](/sharepoint/control-lists)</span><span class="sxs-lookup"><span data-stu-id="4bef7-113">For more information about settings for Microsoft Lists, see [Control settings for Microsoft Lists](/sharepoint/control-lists).</span></span>