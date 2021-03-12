---
title: 1:1 snimanje poziva
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
ms.openlocfilehash: af09e8805409446a42a62c82aa577ad27f09a17a
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/11/2021
ms.locfileid: "50733863"
---
# <a name="11-call-recording"></a><span data-ttu-id="28003-102">1:1 snimanje poziva</span><span class="sxs-lookup"><span data-stu-id="28003-102">1:1 call recording</span></span>

<span data-ttu-id="28003-103">Administratori sada treba da preduzmu korake da bi nastavili da omogućavaju korisnicima da snimaju 1:1 pozive.</span><span class="sxs-lookup"><span data-stu-id="28003-103">Administrators need to take action now to continue allowing users to Record 1:1 calls.</span></span>
 
<span data-ttu-id="28003-104">Počevši od 2012, 2021, počinjemo da sprovodimo nove timove koji pozivaju *na opciju*</span><span class="sxs-lookup"><span data-stu-id="28003-104">Beginning April 12, 2021, we will start enforcing a new Teams Calling Policy option *AllowCloudRecordingForCalls*.</span></span> 

<span data-ttu-id="28003-105">Trenutno 1:1 mogućnosti snimanja poziva kontroliše se opcija *Allowda Drekording* u smernicama timova za sastanak.</span><span class="sxs-lookup"><span data-stu-id="28003-105">Currently 1:1 call recording capabilities are controlled by the *AllowCloudRecording* option in Teams Meeting Policies.</span></span> <span data-ttu-id="28003-106">Ako je korisnicima dozvoljeno da snimaju sastanke tima, takođe mogu da snime 1:1 pozive.</span><span class="sxs-lookup"><span data-stu-id="28003-106">If your users are allowed to record Teams Meetings they can also record 1:1 calls.</span></span>

<span data-ttu-id="28003-107">Ako želite da blokirate sve korisnike da snimaju 1:1 pozive, ne morate da preduzimate nikakve radnje.</span><span class="sxs-lookup"><span data-stu-id="28003-107">If you prefer to block all users from recording 1:1 calls, you do not need to take any action.</span></span> <span data-ttu-id="28003-108">Opcija *Allowza Drecordingforpozivi* će podrazumevano biti $FALSE.</span><span class="sxs-lookup"><span data-stu-id="28003-108">*AllowCloudRecordingForCalls* calling policy option will be $False by default.</span></span>

<span data-ttu-id="28003-109">Ova promena je dokumentovana u sledećem objavljenoj centru za poruke: [(ažurirano) 1:1 Call smernice za zapisivanje smernica](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796) za postavljanje opcije "timovi za pozivanje" morate da koristite [PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-install).</span><span class="sxs-lookup"><span data-stu-id="28003-109">This change is documented in the following Message Center Post: [(Updated) 1:1 Call recording policy introduction](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796) To set the Teams Calling Policy Option you must use [Teams PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-install).</span></span>

<span data-ttu-id="28003-110">**Da biste omogućili snimanje poziva u 1:1 pozivima:** Set-CsTeamsCallingPolicy-opšti identitet $TRUE</span><span class="sxs-lookup"><span data-stu-id="28003-110">**To enable call recording in 1:1 calls:** Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True</span></span>

<span data-ttu-id="28003-111">**Da biste onemogućili snimanje poziva u 1:1 pozivima:** $FALSE Set-CsTeamsCallingPolicy</span><span class="sxs-lookup"><span data-stu-id="28003-111">**To disable call recording in 1:1 calls:** Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $False</span></span>

