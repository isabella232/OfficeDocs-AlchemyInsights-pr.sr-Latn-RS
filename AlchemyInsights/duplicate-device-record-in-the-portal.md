---
title: Duplirani zapis uređaja u portalu
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
- "9001495"
- "4386"
ms.openlocfilehash: 7eb642f85f437fe216c49ce6b060c9061b477629fbd45f50ca0ef315b8cd32d3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "54004168"
---
# <a name="duplicate-device-record-in-the-portal"></a>Duplirani zapis uređaja u portalu

Možda ćete videti 2 zapisa za uređaj na portalu ako uređaj ne prijavi tačno prijavljivanje statusa za saradnju na sajt upravljača konfigurisanja. Da biste proverili status koordinatora uređaja, pregledajte  kolonu za uređaj u alatki "Upravljač konfigurisanja" u okviru Konzola za upravljanje. Ako kolona nije vidljiva, možete da je dodate tako što ćete kliknuti desnim tasterom miša na bilo koje zaglavlja kolona i odabrati ga sa liste.

Zajednički kontrolisana vrednost mora da bude **Da**. Ako je vrednost **Ne**, otvorite aplet za Menadžer konfigurisanja klijenta na uređaju klijenta i potvrdite izbor u polju za potvrdu **Saradništvo** na kartici Opšte.

- Ako je vrednost **omogućena**, to ukazuje na probleme sa komunikacijom klijenta uz management Point. Pregledajte **CcmMessaging. log** na uređaju da biste istražili potencijalne probleme sa povezivanjem.

- Ako je vrednost **onemogućena**, a uređaj je upisan u Intune, uverite se da je uređaj primio smernice za saradnju tako što će pregledati **CoManagementHandler.log** na uređaju.
