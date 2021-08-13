---
title: Uputstva za skrivanje/otkrij grupu sa spiska adresa
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "3161"
ms.openlocfilehash: af7085890d295cf0c41e11aaf18e404313413100cb8a1134bfac051d5fa26996
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "53926259"
---
# <a name="hide-microsoft-365-group-from-address-list-gal"></a>Skrivanje Microsoft 365 iz spiska adresa (GAL)

Da biste sakrili Microsoft 365 sa lista adresa (GAL) Exchange klijenata (kao što su Outlook ili OWA), koristite sledeću komandu u programu EXO shell:

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

Da biste sakrili Microsoft 365 vidljivost grupe Exchange klijentima, koristite sledeću komandu u EXO shell-u:

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

