---
title: Poruke poslate Microsoft 365 grupi nisu primili svi članovi
ms.author: pebaum
author: pebaum
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
- "5995"
ms.openlocfilehash: 29adc5a7b8b74280cb3fcd6369dc4fc3a3e8e957
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/15/2021
ms.locfileid: "51823801"
---
# <a name="messages-sent-to-a-microsoft-365-group-are-not-received-by-all-members"></a>Poruke poslate Microsoft 365 grupi nisu primili svi članovi

Postarajte se da su se svi članovi grupe pretplatili da primaju e-poruke. Pogledajte [Prati grupu u programu Outlook](https://support.microsoft.com/office/e147fc19-f548-4cd2-834f-80c6235b7c36).  

Da biste proverili status poruke članova koji su se pretplatili na grupne e-poruke, pokrenite sledeću komandu [EXO PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps&preserve-view=true):

`Get-UnifiedGroup <GroupName> | Get-UnifiedGroupLinks -LinkType Subscribers`

Koristite sledeću EXO PowerShell komandu da biste konfigurisali sve članove grupe da dobiju e-poruke poslate Microsoft 365 grupi u njihovo poštansko sanduče:

`$Group = "Address of [Microsoft 365 Groups]"Get-UnifiedGroupLinks $Group -LinkType Member | % {Add-UnifiedGroupLinks -Identity $Group -LinkType subscriber -Links $_.Guid.toString() -Confirm:$false}`

Na primer:

`$Group = "testg@contoso.onmicrosoft.com"Get-UnifiedGroupLinks $Group -LinkType Member | % {Add-UnifiedGroupLinks -Identity $Group -LinkType subscriber -Links $_.Guid.toString() -Confirm:$false}`