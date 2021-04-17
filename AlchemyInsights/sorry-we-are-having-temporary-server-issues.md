---
title: Popravljanje Microsoft 365 aplikacija Žao nam je, imamo poruku o privremenim problemima sa serverom
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
- "3420"
- "9001430"
ms.openlocfilehash: 0adf1d66869051b9dd8290ef3466ef9b13aa2d41
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/15/2021
ms.locfileid: "51835285"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a>Rešavanje poruke "Žao nam je, imamo privremene probleme sa serverom" za Microsoft 365 aplikacije

Ako primite ovu poruku, pokušajte sledeće:

1. Proverite postavke zaštitnog zida, antivirusnog softvera i proxy servera da biste potvrdili da ne blokiraju pristup internetu Microsoft 365 aplikacijama. Pogledajte [UL adrese i opsege IP adresa](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. Idite na **Start**  >  **Run**, a zatim **otkucajte services.msc**. Uverite se da su sve sledeće usluge pokrenute:
    - Automatsko podešavanje uređaja koji su povezani sa mrežom
    - Usluga "Lista mreža"
    - Svest o mrežnoj lokaciji
    - Windows evidencija događaja

Ako jedna od ovih usluga nije pokrenuta, pokušajte da je pokrenete. Ako imate problema sa pokretanjem usluge, pokrenite sledeću komandu tako što ćete otvoriti komandnu liniju sa punim dozvolama:

**sfc /scannow**

Kada se ova komanda završi, ponovo pokrenite računar.

Detaljne informacije potražite u [temi "Žao nam je, ne možemo da se povežemo sa vašim nalogom. Greška "Pokušajte ponovo kasnije" prilikom aktiviranja.](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)