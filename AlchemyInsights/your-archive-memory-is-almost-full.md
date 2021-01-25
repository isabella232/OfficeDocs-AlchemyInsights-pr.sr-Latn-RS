---
title: Poštansko sanduče arhive je gotovo popunjeno
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100006"
- "7960"
ms.openlocfilehash: 5c7081f8991716a8ac72f462c6c7ef88e800ab9c
ms.sourcegitcommit: 6f1af4aed507d4c074c36d77666cf00100efe168
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974662"
---
# <a name="your-archive-mailbox-is-almost-full"></a><span data-ttu-id="607ab-102">Poštansko sanduče arhive je gotovo popunjeno</span><span class="sxs-lookup"><span data-stu-id="607ab-102">Your archive mailbox is almost full</span></span>

<span data-ttu-id="607ab-103">Ako korisnik prima upozorenje; **Poštansko sanduče arhive je gotovo popunjeno** ili treba da povećate veličinu njihovog poštanskog sandučeta, evo nekih saveta:</span><span class="sxs-lookup"><span data-stu-id="607ab-103">If the user receives the warning; **Your archive mailbox is almost full**, or you need to increase the size of their archive mailbox, here are some tips:</span></span>

1. <span data-ttu-id="607ab-104">Ako je korisniku dodeljen Exchange online plan 1, nadogradite licencu **online plan 2** da biste povećali veličinu od 50 GB do 100gb.</span><span class="sxs-lookup"><span data-stu-id="607ab-104">If the user is assigned an Exchange Online Plan 1, upgrade to **Exchange Online Plan 2** license to increase the size from 50 GB to 100GB.</span></span>
1. <span data-ttu-id="607ab-105">Ako je korisniku već dodeljen neki od sledećih radnji: **Exchange online plan 2** ili Exchange online plan 1 pomoću programskog dodatka Exchange online arhiv za arhiviranje, koristite dolenavedene korake da biste omogućili automatsko proširivanje:.</span><span class="sxs-lookup"><span data-stu-id="607ab-105">If the user is already assigned either of the following: **Exchange Online Plan 2** or an Exchange Online Plan 1 with an Exchange Online Archiving add-on, use the steps below to enable Auto-Expanding archiving:.</span></span>
 
    1. <span data-ttu-id="607ab-106">[Povezivanje sa uslugom Exchange online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true).</span><span class="sxs-lookup"><span data-stu-id="607ab-106">[Connect to Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true).</span></span>
    2. <span data-ttu-id="607ab-107">Koristite sledeće zapovesti za korisnika:  `Enable-Mailbox <user mailbox> -AutoExpandingArchive`</span><span class="sxs-lookup"><span data-stu-id="607ab-107">Run the following commandlet for the user:  `Enable-Mailbox <user mailbox> -AutoExpandingArchive`</span></span>
    1. <span data-ttu-id="607ab-108">Uradite sledeće zapovjeli da biste potvrdili da je omogućena za korisnika:  `Get-Mailbox <user mailbox> | FL AutoExpandingArchiveEnabled`</span><span class="sxs-lookup"><span data-stu-id="607ab-108">Run the following commandlet to confirm it is enabled for the user:  `Get-Mailbox <user mailbox> | FL AutoExpandingArchiveEnabled`</span></span>

<span data-ttu-id="607ab-109">Više informacija potražite u članku:</span><span class="sxs-lookup"><span data-stu-id="607ab-109">For more information see:</span></span>

- [<span data-ttu-id="607ab-110"> Omogućavanje neograničene arhiviranja-administratorske pomoći-Microsoft 365 usaglašenost | Microsoft docs</span><span class="sxs-lookup"><span data-stu-id="607ab-110"> Enable unlimited archiving - Admin Help - Microsoft 365 Compliance | Microsoft Docs</span></span>](https://docs.microsoft.com/microsoft-365/compliance/enable-unlimited-archiving?view=o365-worldwide&preserve-view=true)

- [<span data-ttu-id="607ab-111">Exchange online ograničenja – opisi usluge | Microsoft docs</span><span class="sxs-lookup"><span data-stu-id="607ab-111">Exchange Online limits - Service Descriptions | Microsoft Docs</span></span>](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits?redirectedfrom=MSDN#storage-limits-across-standalone-plans)

- [<span data-ttu-id="607ab-112">Nadogradnja na drugačiji poslovni plan | Microsoft docs</span><span class="sxs-lookup"><span data-stu-id="607ab-112">Upgrade to a different business plan | Microsoft Docs</span></span>](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan?view=o365-worldwide&preserve-view=true)

