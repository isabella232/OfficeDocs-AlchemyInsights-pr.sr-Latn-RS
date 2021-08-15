---
title: Greške pri sinhronizaciji Apple automatskog unošenja uređaja
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
ms.openlocfilehash: 1664a26b313c4a38c9c6d78cdb89997749ba175fd3dd72f278e99bbd50b0ee84
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "54013762"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a>Greške pri sinhronizaciji Apple automatskog unošenja uređaja

"Otkrili smo da imate jedan ili više ADE/DEP tokena koji su u stanju greške. Dok se stanje greške ne razreši za svaki token na koji token utiče, funkcionalnost ADE neće raditi na očekivani način.".

Ova greška se može prikazati na mnogo načina, uključujući:

1. Uređaji se možda ne sinhronizuju sa ABM/ASM sa aplikacijom Intune
2. Dodele profila za unošenje profila možda neće uspeti
3. Uređaji možda neće uspešno dovršiti ADE unošenje

Proverite da li je greška pri sinhronizaciji prijavljena na Intune konzoli u okviru Uređaji > Upis uređaje > upis u Apple > **tokene programa** za upisovanje .

Jedan od najčešćih uzroka greške pri sinhronizaciji jeste istek trenutnog tokena. U mnogim slučajevima, obnova tokena na koji token utiče rešiće problem.

Ako je istekao rok važenja nekih tokena, pogledajte sledeću dokumentaciju koja će vam pomoći da ih obnovite po pogodan način:

[Obnavljanje automatizovanog tokena unošenja uređaja](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment-program-enroll-ios#renew-an-automated-device-enrollment-token)

Pored toga, možete da vidite sledeću dokumentaciju da biste videli potencijalne načine za druge greške koje izazivaju greške u sinhronizaciji tokena:

[Greške pri ABM/ASM sinhronizaciji za iOS/iPadOS i macOS automatizovane tokene za unošenje uređaja](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#sync-token-errors-between-intune-and-ade-dep)







[Greške pri ABM/ASM sinhronizaciji za iOS/iPadOS i macOS automatizovane tokene za unošenje uređaja](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
