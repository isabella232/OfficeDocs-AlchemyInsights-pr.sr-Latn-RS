---
title: Uputstva za skrivanje/otkrivanje grupe iz liste adresa
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1200024"
- "3161"
ms.openlocfilehash: 02368d6a06df90d76ee1bd5448819e7ffe12c18c
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 06/05/2020
ms.locfileid: "44580023"
---
# <a name="hide-microsoft-365-group-from-address-list-gal"></a>Sakrij Microsoft 365 grupu sa spiska adresa (GAL)

Da biste sakrili Microsoft 365 grupu sa lista adresa (GAL) Exchange klijenata (kao što su Outlook ili OWOVA), koristite sledeću komandu u EXO Shell:

`Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:$true`

Da biste sakrili Microsoft 365 grupu koja je vidljiva za Exchange klijente, koristite sledeću komandu u EXO Shell:

`Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:$true
Check this article for detailed instructions`

