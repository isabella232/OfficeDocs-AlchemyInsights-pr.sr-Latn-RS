---
title: Automatsko čišćenje zastareli uređaja u Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1285"
- "6700008"
ms.openlocfilehash: 874ee290c59df3b5de1421369484a1a5a0ff7be4
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 07/28/2020
ms.locfileid: "46555732"
---
# <a name="automatic-cleanup-of-stale-devices-in-intune"></a>Automatsko čišćenje zastareli uređaja u Intune

Intune dozvoljava administratoru da konfiguriše vremenski interval između 90 i 270 dana, nakon čega se zastareli uređaji uklanjaju iz usluge. Ova postavka je široka organizacija i nakon aktiviranja odmah stupa na snagu. Svi uređaji koji nisu prijavljeni na server Intune za period koji premašuje postavku biće trajno izbrisani.

**Belešku** Samo su objekti MDM uređaja prikladni za ovu radnju čišćenja. EAS samo objekti uređaja su isključeni.

Za dodatne informacije o tome kada uređaj postaje podesan za brisanje na osnovu postavke čišćenja uređaja i njenog "stanja":

Postavka: **Izbriši uređaje posle poslednjeg datuma provere: da (neka vrednost (N) u navedenim danima)**

- Na osnovu vrednosti (N) konfigurisanog u postavci, usluga Intune briše uređaj u navedenim danima nakon što je poslednji put uspešno provjeren.

Postavka: **Izbriši uređaje posle poslednjeg datuma provere: ne**

- 180 dana nakon isteka certifikata uređaja i ne obnavlja se, uređaj se briše.

**Belešku** U oba slučaja uređaj mora biti uspešno registrovan u usluzi Intune. Registracija se javlja tokom prvog uređaja koji se odvija uz uslugu Intune.

Ako se uređaj uspešno registruje za Intune i ne postane registrovan, uređaj se briše 270 dana nakon upisa. (90 dana za označavanje uređaja kao opozvanih, a zatim još 180 dana za brisanje zapisa.)

Nijedan mehanizam trenutno ne postoji u alatki Intune da bi se uspostavio rok važenja certifikacije uređaja za neki dati uređaj.