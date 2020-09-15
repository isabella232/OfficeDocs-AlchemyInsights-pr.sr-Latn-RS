---
title: Uputstva za skrivanje/otkrivanje grupe iz spiska adresa
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "3161"
ms.openlocfilehash: 1ad9ab294d46ca0fc88a454e3503ddcf80398896
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663023"
---
# <a name="hide-microsoft-365-group-from-address-list-gal"></a>Skrivanje Microsoft 365 grupe iz spiska adresa (GAL)

Da biste sakrili Microsoft 365 grupu iz liste adresa (GAL) Exchange klijenta (kao što je Outlook ili OWA), koristite sledeću komandu u EXO Shell:

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

Da biste sakrili Microsoft 365 grupu od vidljive razmene klijenata, koristite sledeću komandu u EXO Shell:

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

