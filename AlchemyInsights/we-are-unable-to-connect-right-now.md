---
title: Problem sa aktivaciju – Trenutno ne možemo da se povežemo
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
- "3408"
- "9001423"
ms.openlocfilehash: 5dad4b43efac2468b57351a4d6c96379ed505071ca144ec0aa518e975633bb18
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "53998176"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a>Popravljanje Microsoft 365 aplikacije "Trenutno ne možemo da se povežemo"

Ako primite ovu poruku, pokušajte sledeće:

1. Proverite postavke zaštitnog zida, antivirusnog softvera i proxy servera da biste potvrdili da ne blokiraju pristup internetu Microsoft 365 aplikacijama. Pogledajte [članak Microsoft opsezi UL adresa i IP adresa.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

2. Idite na **Start**  >  **Run**, a zatim **otkucajte services.msc**. Uverite se da su sve sledeće usluge pokrenute:
    - Automatsko podešavanje uređaja koji su povezani sa mrežom
    - Usluga "Lista mreža"
    - Svest o mrežnoj lokaciji
    - Windows Evidencija događaja

Ako jedna od ovih usluga nije pokrenuta, pokušajte da je pokrenete. Ako imate problema sa pokretanjem usluge, pokrenite sledeću komandu tako što ćete otvoriti komandnu liniju sa punim dozvolama:

**sfc /scannow**

Kada se ova komanda završi, ponovo pokrenite računar.

Detaljne informacije potražite u [temi "Žao nam je, ne možemo da se povežemo sa vašim nalogom. Greška "Pokušajte ponovo kasnije" kada aktivirate ovu Kancelarija sa Microsoft 365.](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)