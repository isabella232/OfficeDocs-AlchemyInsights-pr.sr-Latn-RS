---
title: Problem sa aktivacijom – trenutno ne možemo da se poveћemo
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
- "3408"
- "9001423"
ms.openlocfilehash: 24fe9910d1715b4f5f7d8d06b1d1344d4b8675bc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47725997"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a>Popravka Microsoft 365 aplikacija "trenutno ne možemo da se poveћemo" poruka

Ako primite ovu poruku, Isprobajte sledeće:

1. Proverite zaštitni zid, antivirusni softver i postavke proxy servera da biste potvrdili da ne blokiraju Internet pristup aplikacijama Microsoft 365. Pogledajte [opsege Microsoft URL adresa i IP adresa](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. Idite na **Start**  >  **Run**, a zatim otkucajte **Services. msc**. Proverite da li su pokrenute sledeće usluge:
    - Automatsko podešavanje mrežnih uređaja koji su povezani sa mrežom
    - Usluga liste na mreži
    - Svest o mrežnoj lokaciji
    - Windows evidencija događaja

Ako jedna od ovih usluga nije pokrenuta, pokušajte da je pokrenete. Ako vam je problem da pokrenete uslugu, pokrenete sledeću komandu tako što ćete otvoriti komandnu liniju sa punim dozvolama:

**Sfc/scannow**

Kada se komanda završi, ponovo pokrenite računar.

Detaljne informacije potražite u članku ["Žao nam je, ne možemo da se poveћemo sa vašim nalogom. Pokušajte ponovo kasnije "Greška prilikom aktiviranja sistema Office sa Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).