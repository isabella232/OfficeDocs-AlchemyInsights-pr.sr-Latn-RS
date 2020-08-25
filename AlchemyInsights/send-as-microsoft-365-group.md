---
title: Pošalji kao Microsoft 365 grupa
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/19/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
ms.openlocfilehash: cfb4bd5ce59eeccdd0812d013b8a444aebeb1d4c
ms.sourcegitcommit: 9818d3c8e6b10f23244e51286e2463caf48fffd5
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/21/2020
ms.locfileid: "46872120"
---
# <a name="send-as-microsoft-365-group"></a><span data-ttu-id="1d06a-102">Pošalji kao Microsoft 365 grupa</span><span class="sxs-lookup"><span data-stu-id="1d06a-102">Send As Microsoft 365 group</span></span>

<span data-ttu-id="1d06a-103">Možete dodeliti dozvole "Pošalji kao" da biste omogućili određenim korisnicima da šalju poruke kao grupu Microsoft 365:</span><span class="sxs-lookup"><span data-stu-id="1d06a-103">You can assign Send As permissions to allow specific users to send messages as a Microsoft 365 group:</span></span>  

1. <span data-ttu-id="1d06a-104">Povezivanje sa uslugom Exchange online PowerShell.</span><span class="sxs-lookup"><span data-stu-id="1d06a-104">Connect to Exchange Online PowerShell.</span></span>  

2. <span data-ttu-id="1d06a-105">Uradite sledeće:</span><span class="sxs-lookup"><span data-stu-id="1d06a-105">Run the following command:</span></span>  

    <span data-ttu-id="1d06a-106">Add-RecipientPermission `<GroupName>` -Poverenit `<MailboxName>` sendas</span><span class="sxs-lookup"><span data-stu-id="1d06a-106">Add-RecipientPermission `<GroupName>` -Trustee `<MailboxName>` -AccessRights SendAs</span></span>

<span data-ttu-id="1d06a-107">Više informacija potražite u članku [Omogućavanje članovima za slanje ili slanje u ime grupe](https://docs.microsoft.com/microsoft-365/admin/create-groups/allow-members-to-send-as-or-send-on-behalf-of-group?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="1d06a-107">For more information, see [Allow members to send as or send on behalf of a group](https://docs.microsoft.com/microsoft-365/admin/create-groups/allow-members-to-send-as-or-send-on-behalf-of-group?view=o365-worldwide).</span></span>