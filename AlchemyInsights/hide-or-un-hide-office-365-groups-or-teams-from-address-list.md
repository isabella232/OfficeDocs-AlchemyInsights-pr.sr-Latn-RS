---
title: Skrivanje ili poništavanje skrivanja Office 365 grupa ili timova sa spiska adresa
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002947"
- "5642"
ms.openlocfilehash: 12e221c69775f3dfeed1781b70d3061e1ca0ac3b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/15/2021
ms.locfileid: "51811470"
---
# <a name="hide-or-un-hide-office-365-groups-or-teams-from-address-list"></a>Skrivanje ili poništavanje skrivanja Office 365 grupa ili timova sa spiska adresa

Koristite sledeću EXO PowerShell komandu da biste sakrili ili poništili skrivanje Office 365 grupe/timova sa spiskova adresa (GAL) Exchange klijenata (Outlook, OWA):

`
    Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:<$true> or <$false>
`

Koristite sledeću EXO PowerShell komandu da biste sakrili ili poništili skrivanje Office365 grupe/timova iz Exchange klijenata (Outlook, OWA):

`
    Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:<$true> or <$false>
`

- Za detaljna uputstva pogledajte [skrivanje Office 365 grupa od GAL-a i Exchange klijenata.](https://docs.microsoft.com/schooldatasync/hide-office-365-groups-from-the-gal)
