---
title: Popravka Microsoft 365 aplikacija Žao nam je, imamo poruku o privremenim serverima
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
- "3420"
- "9001430"
ms.openlocfilehash: e00504d318efdea4968ddf98b3ce9591f8993e38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47758259"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a>Popravka Microsoft 365 aplikacija "Žao nam je, imamo trenutne probleme sa serverom"

Ako primite ovu poruku, Isprobajte sledeće:

1. Proverite zaštitni zid, antivirusni softver i postavke proxy servera da biste potvrdili da ne blokiraju Internet pristup aplikacijama Microsoft 365. Pogledajte [opseg URL adresa i IP adresa](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. Idite na **Start**  >  **Run**, a zatim otkucajte **Services. msc**. Proverite da li su pokrenute sledeće usluge:
    - Automatsko podešavanje mrežnih uređaja koji su povezani sa mrežom
    - Usluga liste na mreži
    - Svest o mrežnoj lokaciji
    - Windows evidencija događaja

Ako jedna od ovih usluga nije pokrenuta, pokušajte da je pokrenete. Ako vam je problem da pokrenete uslugu, pokrenete sledeću komandu tako što ćete otvoriti komandnu liniju sa punim dozvolama:

**Sfc/scannow**

Kada se komanda završi, ponovo pokrenite računar.

Detaljne informacije potražite u članku ["Žao nam je, ne možemo da se poveћemo sa vašim nalogom. Pokušajte ponovo kasnije "Greška prilikom aktiviranja](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).