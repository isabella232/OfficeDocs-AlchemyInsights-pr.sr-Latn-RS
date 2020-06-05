---
title: Pitanje aktivacije-ne možemo odmah da se povežemo
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3408"
- "9001423"
ms.openlocfilehash: b46bac60633ad9a006b9446919b8c99e221b07e4
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 06/05/2020
ms.locfileid: "44581889"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a>Popravljanje Microsoft 365 aplikacija "Trenutno nismo u mogućnosti da se povežemo" poruka

Ako dobijete ovu poruku, pokušajte sledeće:

1. Proverite zaštitni zid, antivirusni softver i proxy postavke da biste potvrdili da ne blokiraju pristup internetu u Microsoft 365 aplikacijama. Pogledajte [Microsoft URL adrese i OPSEGE IP adresa](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. Idite na **početni ekran**  >  **Run**i otkucajte **usluge. msc**. Uverite se da su sve pokrenute sledeće usluge:
    - Automatsko podešavanje uređaja povezanih sa mrežom
    - Usluga liste mreža
    - Svest o mrežnoj lokaciji
    - Windows evidencija događaja

Ako neka od ovih usluga nije pokrenuta, pokušajte da ga pokrenete. Ako imate problem sa pokretanjem usluge, pokrenite sledeću komandu tako što ćete otvoriti komandnu liniju sa punim dozvolama:

**Sfc/scannow**

Nakon završetka ove komande, ponovo pokrenite računar.

Detaljnije informacije potražite u članku ["Nažalost, ne možemo da se povežemo sa vašim nalogom. Pokušajte ponovo kasnije "greška kada aktivirate Office sa Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).