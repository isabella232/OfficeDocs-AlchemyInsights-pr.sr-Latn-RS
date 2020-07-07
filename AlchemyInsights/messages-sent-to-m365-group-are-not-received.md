---
title: Poruke poslate Microsoft 365 grupi ne primaju svi članovi
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
- "5995"
ms.openlocfilehash: 2c98841aaa278c1bc18b3ec9007240b1e856f41e
ms.sourcegitcommit: 743a9e4967993c5463272240280c22e27a8dc5b6
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 07/06/2020
ms.locfileid: "45051515"
---
# <a name="messages-sent-to-a-microsoft-365-group-are-not-received-by-all-members"></a>Poruke poslate u Microsoft 365 grupu ne primaju svi članovi

Uverite se da su svi članovi grupe pretplaćeni da bi primili e-poruke. Pogledajte odeljak [Praćenje grupe u programu Outlook](https://support.microsoft.com/office/e147fc19-f548-4cd2-834f-80c6235b7c36).  

Da biste proverili status poruke članova koji su pretplaćeni da grupišu e-poruke, pokrenite sledeću komandu na [Exo PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell?view=exchange-ps):

`Get-UnifiedGroup <GroupName> | Get-UnifiedGroupLinks -LinkType Subscribers`