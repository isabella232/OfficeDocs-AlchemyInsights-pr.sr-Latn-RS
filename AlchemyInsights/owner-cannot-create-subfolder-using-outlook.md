---
title: Vlasnik ne može da kreira podfasciklu pomoću programa Outlook
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5884"
- "3500007"
ms.openlocfilehash: 2116bb837e4378ea29d7882df1d3010b3a4e0b1c
ms.sourcegitcommit: 936330b11fec49f6174eadea6c765bdf9e6ba784
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 06/12/2020
ms.locfileid: "44749143"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a><span data-ttu-id="4ae99-102">Vlasnik ne može da kreira podfasciklu pomoću programa Outlook</span><span class="sxs-lookup"><span data-stu-id="4ae99-102">Owner cannot create sub-folder using Outlook</span></span>

<span data-ttu-id="4ae99-103">**Postoji problem sa vlasnicima javnih fascikli koji kreiraju potfascikle pomoću programa Outlook. To pitanje će uskoro biti ispravljeno.**</span><span class="sxs-lookup"><span data-stu-id="4ae99-103">**There's an ongoing issue with public folder owners creating subfolders using Outlook. The issue will be fixed soon.**</span></span>

<span data-ttu-id="4ae99-104">U međuvremenu, koristite jedno od sledećih rešenja:</span><span class="sxs-lookup"><span data-stu-id="4ae99-104">Meanwhile, use one of the following workarounds:</span></span>

1. <span data-ttu-id="4ae99-105">Korišćenje programa Outlook za MAC za kreiranje potfascikle dok problem utiče samo na Outlook za prozore radne površine (sve verzije)</span><span class="sxs-lookup"><span data-stu-id="4ae99-105">Use Outlook for MAC to create the subfolder as the issue impacts only Outlook for desktop windows (all versions)</span></span>
2. <span data-ttu-id="4ae99-106">Neka admin napravi potfasciklu koristeći "EXO Shell" ili EAC</span><span class="sxs-lookup"><span data-stu-id="4ae99-106">Have admin create the subfolder using EXO Shell or EAC</span></span>
3. <span data-ttu-id="4ae99-107">Promenite DefaultPublicFolderMailbox/EffectivePublicFolderMailbox za korisnika u drugo poštansko sanduče nego poštansko sanduče sadržaja za fasciklu koja uzrokuje problem</span><span class="sxs-lookup"><span data-stu-id="4ae99-107">Change the DefaultPublicFolderMailbox/EffectivePublicFolderMailbox on the user to other mailbox than the Content Mailbox for the folder causing issue</span></span>  
    - <span data-ttu-id="4ae99-108">*Set-poštansko sanduče User1 DefaultPublicFolderMailbox PubMBX3*</span><span class="sxs-lookup"><span data-stu-id="4ae99-108">*Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*</span></span>
4. <span data-ttu-id="4ae99-109">Sačekajte sat, ponovo pokrenite Outlook Client</span><span class="sxs-lookup"><span data-stu-id="4ae99-109">Wait for an hour, restart outlook client</span></span>