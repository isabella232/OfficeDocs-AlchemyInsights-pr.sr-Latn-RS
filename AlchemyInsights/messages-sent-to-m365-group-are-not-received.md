---
title: Poruke poslate Microsoft 365 grupi nisu primili svi članovi
ms.author: pebaum
author: pebaum
manager: mnirkhe
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
- "5995"
ms.openlocfilehash: 39a4f8115a4742947b3e6394396be5ce3b01e772
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: HT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/04/2021
ms.locfileid: "50430697"
---
# <a name="messages-sent-to-a-microsoft-365-group-are-not-received-by-all-members"></a><span data-ttu-id="23bea-102">Poruke poslate Microsoft 365 grupi nisu primili svi članovi</span><span class="sxs-lookup"><span data-stu-id="23bea-102">Messages sent to a Microsoft 365 group are not received by all members</span></span>

<span data-ttu-id="23bea-103">Uverite se da su se svi članovi grupe pretplatili da primaju e-poruke.</span><span class="sxs-lookup"><span data-stu-id="23bea-103">Make sure that all group members have subscribed to receive the emails.</span></span> <span data-ttu-id="23bea-104">Pogledajte [Prati grupu u programu Outlook](https://support.microsoft.com/office/e147fc19-f548-4cd2-834f-80c6235b7c36).</span><span class="sxs-lookup"><span data-stu-id="23bea-104">See [Follow a group in Outlook](https://support.microsoft.com/office/e147fc19-f548-4cd2-834f-80c6235b7c36).</span></span>  

<span data-ttu-id="23bea-105">Da biste proverili status poruke članova koji su se pretplatili na grupne e-poruke, pokrenite sledeću komandu [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true):</span><span class="sxs-lookup"><span data-stu-id="23bea-105">To check the message status of members who have subscribed to group emails, run the following command on [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true):</span></span>

`Get-UnifiedGroup <GroupName> | Get-UnifiedGroupLinks -LinkType Subscribers`

<span data-ttu-id="23bea-106">Koristite sledeću EXO PowerShell komandu da biste konfigurisali sve članove grupe da dobiju e-poruke poslate Microsoft 365 grupi u njihovo poštansko sanduče:</span><span class="sxs-lookup"><span data-stu-id="23bea-106">Use the following EXO PowerShell command to configure all group members to receive emails sent to Microsoft 365 group in their inbox:</span></span>

`$Group = "Address of [Microsoft 365 Groups]"Get-UnifiedGroupLinks $Group -LinkType Member | % {Add-UnifiedGroupLinks -Identity $Group -LinkType subscriber -Links $_.Guid.toString() -Confirm:$false}`