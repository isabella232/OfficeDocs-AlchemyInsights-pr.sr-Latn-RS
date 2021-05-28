---
title: 1:1 snimak poziva
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/18/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002530"
- "7648"
ms.openlocfilehash: 18c68fee514681b2a81c3cfa022c29ce83834f22
ms.sourcegitcommit: 610a5d950cdf488870601762ef52d881e3e22a48
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 05/28/2021
ms.locfileid: "52696972"
---
# <a name="11-call-recording"></a><span data-ttu-id="1a5ec-102">1:1 snimak poziva</span><span class="sxs-lookup"><span data-stu-id="1a5ec-102">1:1 call recording</span></span>

<span data-ttu-id="1a5ec-103">Ako je **dugme Započni** snimanje zasivo u pozivu 1:1, morate da promenite postavke smernica za korisnika na koje ovo utiče.</span><span class="sxs-lookup"><span data-stu-id="1a5ec-103">If the **Start Recording** button is grayed out in a 1:1 call, you need to change the policy settings for the impacted user.</span></span>   

<span data-ttu-id="1a5ec-104">Počejući od 31. maja 2021. počećemo da nalažemo nove smernice za Teams smernica za pozivanje *AllowCloudRecordingForCalls.*</span><span class="sxs-lookup"><span data-stu-id="1a5ec-104">Beginning May 31, 2021, we'll start enforcing a new Teams Calling Policy *AllowCloudRecordingForCalls*.</span></span> <span data-ttu-id="1a5ec-105">Pre ove promene, snimanje poziva 1:1 kontroliše *AllowCloudRecording* Teams za sastanke.</span><span class="sxs-lookup"><span data-stu-id="1a5ec-105">Prior to this change, 1:1 call recording is controlled by the *AllowCloudRecording* Teams Meeting Policy.</span></span> <span data-ttu-id="1a5ec-106">Ova promena je dokumentovana u objavi centra za poruke: [(Ažurirano) 1:1](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796)Uvod u smernice za snimanje poziva .</span><span class="sxs-lookup"><span data-stu-id="1a5ec-106">This change is documented in the Message Center post: [(Updated) 1:1 Call recording policy introduction](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796).</span></span>  

<span data-ttu-id="1a5ec-107">*AllowCloudRecordingForCalls*   opcija smernica pozivanja je **podrazumevano $False** podešena na vrednost .</span><span class="sxs-lookup"><span data-stu-id="1a5ec-107">*AllowCloudRecordingForCalls* calling policy option is set to **$False** by default.</span></span> <span data-ttu-id="1a5ec-108">Ako biste radije da blokirate svim korisnicima snimanje 1:1 poziva, ne morate ništa da preduzmete.</span><span class="sxs-lookup"><span data-stu-id="1a5ec-108">If you prefer to block all users from recording 1:1 calls, you don't need to take any action.</span></span>  

<span data-ttu-id="1a5ec-109">Da biste omogućili snimanje poziva za sve korisnike u 1:1 pozivima koristite Teams PowerShell da biste pokrenite sledeću cmdlet Teams</span><span class="sxs-lookup"><span data-stu-id="1a5ec-109">To enable call recording for all users in 1:1 calls use Teams PowerShell to run the following cmdlet:</span></span> 

<span data-ttu-id="1a5ec-110">**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True**</span><span class="sxs-lookup"><span data-stu-id="1a5ec-110">**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True**</span></span> 

<span data-ttu-id="1a5ec-111">Druga mogućnost je da kreirate nove smernice i postavite **-AllowCloudRecordingForCalls** **da $true** te smernice dodelili korisnicima.</span><span class="sxs-lookup"><span data-stu-id="1a5ec-111">Alternatively, you can create a new policy and set **-AllowCloudRecordingForCalls** to **$true** and assign that policy to your users.</span></span> 

<span data-ttu-id="1a5ec-112">Više informacija potražite u 1:1 Kontrole smernica za snimanje poziva [su (Gotovo!) Ovde](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668).</span><span class="sxs-lookup"><span data-stu-id="1a5ec-112">For more information, see [1:1 Call Recording Policy Controls Are (Almost!) Here](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668).</span></span>
