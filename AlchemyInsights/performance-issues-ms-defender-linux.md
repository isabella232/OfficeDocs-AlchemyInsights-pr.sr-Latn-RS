---
title: Problemi sa performansama za Microsoft zaštitnik za krajnju tačku na Linux
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11491"
- "9001464"
ms.openlocfilehash: 268f44640d3b2d8764133560d0cbf500eb4afd22
ms.sourcegitcommit: 8242a824491f64be48dfe81da09766920fbd7feb
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 06/06/2021
ms.locfileid: "52794227"
---
# <a name="performance-issues-for-microsoft-defender-for-endpoint-on-linux"></a>Problemi sa performansama za Microsoft zaštitnik za krajnju tačku na Linux

Ovaj članak vas vodi kroz korake za identifikovanje problema sa performansama za Microsoft zaštitnik za krajnju tačku na linux-u.

Važno je prvo da proverite da li je problem koji imate rešen u najnovijoj [verziji.](/microsoft-365/security/defender-endpoint/linux-whatsnew) 

Da biste započeli istraživanje, pogledajte [članak Rešavanje problema sa performansama za Microsoft zaštitnik za krajnju tačku na Linux.](/microsoft-365/security/defender-endpoint/linux-support-perf)

## <a name="exclusions"></a>Izusci

Izusvi mogu da vam pomognu da ublažite probleme sa performansama. Pregledajte izuzetke pre nego što počnete kako bi dodatni rizik bio poznat i dokumentovan.

Više informacija potražite u članku Konfigurisanje izuzetka i provera valjanosti izuzetka za Microsoft zaštitnik za [krajnju tačku na linux-u.](/microsoft-365/security/defender-endpoint/linux-exclusions)

Kada imate više datoteka koje & izuzmu, a sve se na istoj planini, možda je lakše isključiti planinu. Počev od februarskog izdanja 101.22.80, možete da isključite celu tačku planine.

Na primer, ako je /mnt/backup tačka planine, možete da dodate /mnt/backup na listu izuzetih stavki tako što ćete pokrenuti ovu komandu:

`$ mdatp exclusion folder add –path /mnt/backup`

**Napomi:** Dodavanje izuzetka povećava rizik od toga da malver nije otkriven i da ga treba sprovesti i primeniti sa brigom.

## <a name="need-help"></a>Potrebna vam je pomoć?

Da biste pomogli na najefikasniji način, prikupite dijagnostične podatke pre nego što otvorite predmet za podršku.
