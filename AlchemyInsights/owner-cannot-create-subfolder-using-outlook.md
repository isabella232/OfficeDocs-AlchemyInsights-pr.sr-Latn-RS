---
title: Vlasnik ne može da kreira potfasciku pomoću programa Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5884"
- "3500007"
ms.openlocfilehash: b2ab7b60bc521fd28d68333bb963528f7b9e05f2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/15/2021
ms.locfileid: "51836149"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a><span data-ttu-id="025bd-102">Vlasnik ne može da kreira potfasciku pomoću programa Outlook</span><span class="sxs-lookup"><span data-stu-id="025bd-102">Owner cannot create sub-folder using Outlook</span></span>

<span data-ttu-id="025bd-103">**Postoji tekući problem sa vlasnicima javnih fascikli koji prave potfascikle pomoću programa Outlook. Problem će uskoro biti rešen.**</span><span class="sxs-lookup"><span data-stu-id="025bd-103">**There's an ongoing issue with public folder owners creating subfolders using Outlook. The issue will be fixed soon.**</span></span>

<span data-ttu-id="025bd-104">U međuvremenu koristite neko od sledećih zaokreta:</span><span class="sxs-lookup"><span data-stu-id="025bd-104">Meanwhile, use one of the following workarounds:</span></span>

1. <span data-ttu-id="025bd-105">Korišćenje programa Outlook za MAC za kreiranje potfascikle jer problem utiče samo na Outlook za windows računare (sve verzije)</span><span class="sxs-lookup"><span data-stu-id="025bd-105">Use Outlook for MAC to create the subfolder as the issue impacts only Outlook for desktop windows (all versions)</span></span>
2. <span data-ttu-id="025bd-106">Kreiranje potfascikle pomoću programa EXO Shell ili EAC</span><span class="sxs-lookup"><span data-stu-id="025bd-106">Have admin create the subfolder using EXO Shell or EAC</span></span>
3. <span data-ttu-id="025bd-107">Promena defaultPublicFolderMailbox/EffectivePublicFolderMailbox korisnika u drugo poštansko sanduče nego poštansko sanduče sadržaja za fasciklu koja uzrokuje problem</span><span class="sxs-lookup"><span data-stu-id="025bd-107">Change the DefaultPublicFolderMailbox/EffectivePublicFolderMailbox on the user to other mailbox than the Content Mailbox for the folder causing issue</span></span>  
    - <span data-ttu-id="025bd-108">*Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*</span><span class="sxs-lookup"><span data-stu-id="025bd-108">*Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*</span></span>
4. <span data-ttu-id="025bd-109">Sačekajte sat vremena, ponovo pokrenite Outlook klijent</span><span class="sxs-lookup"><span data-stu-id="025bd-109">Wait for an hour, restart outlook client</span></span>