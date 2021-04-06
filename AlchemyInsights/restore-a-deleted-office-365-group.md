---
title: Vraćanje izbrisane Microsoft 365 grupe
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "98"
- "1200024"
ms.assetid: bc0396ea-c426-4d1d-bb89-ced602d06fb6
ms.openlocfilehash: caa2c8987eecb89bac3469bf9471847858cab0ba
ms.sourcegitcommit: ec99a3a2e1e6a13d9a829d65ad1692a607dc3a17
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/06/2021
ms.locfileid: "51597457"
---
# <a name="restore-a-deleted-microsoft-365-group"></a><span data-ttu-id="469e6-102">Vraćanje izbrisane Microsoft 365 grupe</span><span class="sxs-lookup"><span data-stu-id="469e6-102">Restore a deleted Microsoft 365 group</span></span>

<span data-ttu-id="469e6-103">Možete da vratite izbrisanu Microsoft 365 grupu ili Microsoft Teams u roku od 30 dana od brisanja.</span><span class="sxs-lookup"><span data-stu-id="469e6-103">You can restore a deleted Microsoft 365 group or Microsoft Teams within 30 days from the deletion.</span></span>

1. <span data-ttu-id="469e6-104">Idite u Microsoft 365 centar za [administaciju](https://aka.ms/RestoreDeletedGroup) da biste se prijavili i naveli izbrisane grupe i timove.</span><span class="sxs-lookup"><span data-stu-id="469e6-104">Go to the [Microsoft 365 admin center](https://aka.ms/RestoreDeletedGroup) to log in and list the deleted groups and teams.</span></span>

    <span data-ttu-id="469e6-105">**Napomogućeno:** Prijavite se pomoću naloga koji je dodeljen administratoru zakupca ili ulozi administratora grupe.</span><span class="sxs-lookup"><span data-stu-id="469e6-105">**Note:** Log in using the account that is assigned to either the tenant administrator or the groups admin role.</span></span>

1. <span data-ttu-id="469e6-106">Izaberite izbrisanu Microsoft 365 grupu/Teams za vraćanje u prethodno stanje i kliknite na vrati **grupu.**</span><span class="sxs-lookup"><span data-stu-id="469e6-106">Select the deleted Microsoft 365 group/Teams to be restored and click **restore group**.</span></span>

    <span data-ttu-id="469e6-107">Ako nije moguće vratiti grupu zbog neusaglašene SMTP adrese, koristite sledeću komandu da biste pronašli objekat koji izaziva neusaglašenost i uklonili SMTP adresu:</span><span class="sxs-lookup"><span data-stu-id="469e6-107">If the group can't be restored because of a conflicting SMTP address, use following command to find the object that’s causing conflict and remove the SMTP address:</span></span>

    `Get-Recipient -Filter "EmailAddresses -eq '<conflictingsmtpaddress>'"`

    <span data-ttu-id="469e6-108">**Napomogućeno:** U nekim slučajevima može biti čak do 24 časa da grupe i svi njeni podaci budu vraćeni u prethodno stanje.</span><span class="sxs-lookup"><span data-stu-id="469e6-108">**Note:** In some cases, it might take as long as 24 hours for the group and all of its data to be restored.</span></span>

    <span data-ttu-id="469e6-109">Dodatne informacije ili da biste saznali kako da vratite grupe u prethodno stanje pomoću programa PowerShell potražite u članku Vraćanje [izbrisane Microsoft 365 grupe.](https://go.microsoft.com/fwlink/?linkid=867802)</span><span class="sxs-lookup"><span data-stu-id="469e6-109">For more info, or to learn how to restore groups using PowerShell, see [Restore a deleted Microsoft 365 group](https://go.microsoft.com/fwlink/?linkid=867802).</span></span>