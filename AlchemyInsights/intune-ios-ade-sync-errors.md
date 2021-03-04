---
title: Funkcija Apple automatskih upisivanja uređaja
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000654"
- "7256"
ms.openlocfilehash: 912c9e56b4c468fb333769f15bd7c212594dc11a
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/04/2021
ms.locfileid: "50448936"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a>Funkcija Apple automatskih upisivanja uređaja

"Otkrili smo da imate neke EJD/DEP simbole koji se nalaze u stanju greške. Dok se stanje greške ne reši za svaki utiču na Token, funkcionalnost Jade neće funkcionisati na očekivani način. ".

Ova greška se može manifestuiti na više načina uključujući:

1. Uređaji se možda neće sinhronizovati sa ABM/Jumom u Intune
2. Dodeljene profile profila možda neće uspeti
3. Uređaji možda neće uspješno dovršiti prijavljivanje

Potvrdite izbor u vidu greške pri sinhronizaciji prijavljene u konzoli Intune u okviru **Uređaji > Enroll uređaji > Apple prijavljivanje > tokena programa** za prijavljivanje.

Jedan od najčešćih uzroka greške pri sinhronizaciji je isticanje trenutnog simbola. U mnogim slučajevima, obnavljanje pogođene oznake rešavaće problem.

Ako je neki od svojih željena istekao, pogledajte sledeću dokumentaciju koja će vam pomoći da ih obnovite po potrebi:

[Obnavljanje simbola automatizovanog upisivanja uređaja](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment-program-enroll-ios#renew-an-automated-device-enrollment-token)

Pored toga, možete da vidite sledeću dokumentaciju da biste videli potencijalne probleme za druge greške koji prouzrokuju greške simbola:

[Greške u sinhronizaciji ABM/Zamsync za iOS/iPadOS i macOS automatski Naupisivanje uređaja](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#sync-token-errors-between-intune-and-ade-dep)







[Greške u sinhronizaciji ABM/Zamsync za iOS/iPadOS i macOS automatski Naupisivanje uređaja](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
