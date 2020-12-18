---
title: Funkcija Apple automatskih upisivanja uređaja
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000654"
- "7256"
ms.openlocfilehash: d7a9398046a1073e30fdbe2950f750bb55d4fa2f
ms.sourcegitcommit: 87c8d0a1e6668211b9dd5427f98984ccdcadb02d
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 12/17/2020
ms.locfileid: "49714977"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a>Funkcija Apple automatskih upisivanja uređaja

"Otkrili smo da imate neke EJD/DEP simbole koji se nalaze u stanju greške. Dok se stanje greške ne reši za svaki utiču na Token, funkcionalnost EJD neće funkcionisati na isti način ".

Ova greška se može manifestuiti na više načina uključujući:

1. Uređaji se možda neće sinhronizovati sa ABM/Jumom u Intune
2. Dodeljene profile profila možda neće uspeti
3. Uređaji možda neće uspješno dovršiti prijavljivanje

Proverite da li je došlo do greške pri sinhronizaciji prijavljene u konzoli Intune u okviru **uređaji > Enroll uređajima > Apple prijavljivanje >** inrouacije programa za prijavljivanje i Redigujte sledeću dokumentaciju da biste videli bilo koji potencijalni sistem oporavka:

[Greške u sinhronizaciji ABM/Zamsync za iOS/iPadOS i macOS automatski Naupisivanje uređaja](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
