---
title: Status senzora krajnje tačke zaštitnika
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/21/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11084"
- "9003537"
ms.openlocfilehash: a53a0109c3b974806d04135dd2c102de81ec560f
ms.sourcegitcommit: ded29f44e5019b1929218b02733b390899843680
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 05/24/2021
ms.locfileid: "52676338"
---
# <a name="defender-endpoint-check-sensor-status"></a>Status senzora krajnje tačke zaštitnika

Pločka **Uređaji sa senzorima** se nalazi na sistemsku tablu "Bezbednosne operacije". Ova pločice pruža informacije o mogućnosti pojedinačnog uređaja da pruži senzorske podatke i komunicira sa uslugom "Zaštitnik za krajnju tačku". On prijavljuje koliko uređaja zahteva pažnju i pomaže vam da identifikujete problematične uređaje i preduzmete radnju kako biste rešili poznate probleme.

Dva indikatora statusa na pločnici pružaju informacije o broju uređaja koji uslugi ne prijavljujete ispravno:

- **Pogrešno konfigurisanje** Uređaji koji možda delimično izveštavaju senzorske podatke u uslugu "Zaštitnik za krajnju tačku" i možda imaju greške u konfiguraciji koje treba da se isprave.
- **Neaktivan** Uređaji koji su prestali da prijavljujeju u uslugu "Zaštitnik za krajnje tačke" više od sedam dana u prošlom mesecu.

Klik na bilo koju grupu će vas usmeriti na listu Uređaji filtrirane u skladu sa svojim izborom. Na listi Uređaji možete da filtrirate listu stanja zdravlja prema sledećem statusu:

- **Aktivno** Uređaji koji aktivno izveštavaju o usluzi "Zaštitnik za krajnju tačku".
- **Pogrešno konfigurisanje** Uređaji koji možda delimično prijavljujeju podatke senzora u uslugu "Zaštitnik za krajnju tačku", ali imaju greške u konfiguraciji koje treba da se isprave. Pogrešno konfigurisani uređaji mogu imati jedan ili kombinaciju sledećih problema:

    - Nema podataka senzora – Uređaji su prestali da šalju podatke senzora. Ograničena upozorenja se mogu aktivirati sa uređaja.
    - Komunikacija sa otežava – Mogućnost komunikacije sa uređajem je uklonjena. Slanje datoteka radi dubinske analize, blokiranje datoteka, izolacija uređaja od mreže i drugih radnji koje zahtevaju komunikaciju sa uređajem možda neće raditi.
- **Neaktivan** Uređaji koji su prestali da prijavljujeju izveštavanje u uslugu "Zaštitnik za krajnje tačke".

Možete da preuzmete celu listu u CSV formatu pomoću funkcije "Izvoz".

Više informacija potražite u članku [Provera stanja zdravstvenog stanja senzora u programu Microsoft zaštitnik za krajnju tačku.](/microsoft-365/security/defender-endpoint/check-sensor-status)

Više informacija o tome šta je izazvalo neaktivnost ili neispravno konfigurisanje uređaja potražite u članku Popravka neispravno skeniranih senzora u programu Microsoft zaštitnik za krajnju [tačku.](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors)
