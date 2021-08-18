---
title: Skrivanje ili skrivanje Office 365 ili timova sa spiska adresa
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
ms.openlocfilehash: 7e667e22cd81f38a1a2c1385bf42e5227cb641480f4b505110ee7349a13f13a1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "54088410"
---
# <a name="hide-or-un-hide-office-365-groups-or-teams-from-address-list"></a>Skrivanje ili skrivanje Office 365 ili timova sa spiska adresa

Koristite sledeću EXO PowerShell komandu da biste sakrili ili Office 365 grupe/timove sa spiskova adresa (GAL) Exchange klijenata (Outlook, OWA):

`
    Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:<$true> or <$false>
`

Koristite sledeću EXO PowerShell komandu da biste sakrili ili poništili skrivanje Office365 grupe/timova od Exchange klijenata (Outlook, OWA):

`
    Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:<$true> or <$false>
`

- Detaljna uputstva pogledajte Office 365 Skrivanje grupa [od GAL-a i Exchange klijenata.](https://docs.microsoft.com/schooldatasync/hide-office-365-groups-from-the-gal)
