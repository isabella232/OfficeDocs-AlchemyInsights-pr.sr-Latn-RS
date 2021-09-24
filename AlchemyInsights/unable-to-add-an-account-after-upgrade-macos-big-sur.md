---
title: Nije moguće dodati nalog posle nadogradnje na macOS 11.6 Big Sur
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 09/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13840"
- "9008627"
ms.openlocfilehash: 91cb402e63b68de4a08f6dcb80807ff2e01300c9
ms.sourcegitcommit: a097d1f8915a31ed8460b5b68dccc8d87e563cc0
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/22/2021
ms.locfileid: "59506755"
---
# <a name="unable-to-add-an-account-after-upgrading-to-macos-116-big-sur"></a>Nije moguće dodati nalog posle nadogradnje na macOS 11.6 Big Sur

Nakon nadogradnje na macOS 11.6, OneDrive nalog za poslovni ili školski nalog ili OneDrive lični nalog možda se neće pojaviti na listi naloga i možda ne možete da se prijavite na drugi nalog iz aplikacije.

Rešenje ovog problema je razvijeno. Prvo utvrdite da li imate OneDrive ili App Store verziju:

- Izaberite oblak OneDrive na traci sa menijima > **Pomoć & Postavke**  >  **Željene postavke**  >  **o**. Ako broj verzije ne uključuje **(standalone),** imate verziju App Store proizvoda.

Ako koristite samostalnu verziju programa OneDrive, ponovo pokrenite računar i OneDrive automatsko ažuriranje u izdanju u kom je ovaj problem rešen. Ako želite ručno da instalirate instalaciju, preuzmite ovu [.zip](https://oneclient.sfx.ms/Mac/Prod/21.170.0822.0003/OneDrive.zip)datoteku , dekompirujte datoteku i kopirajte OneDrive aplikaciju u fasciklu Aplikacije (tako što ćete zameniti postojeću OneDrive aplikaciju).

Ako koristite verziju App Store, razmotrite instaliranje OneDrive. Ova verzija radi na isti način kao i verzija usluge App Store, ali omogućava korporaciji Microsoft da brže ponudi ispravke korisnicima i povezuje ih sa verzijom koja uključuje rešenje ovog problema.

1. Preuzmite OneDrive verziju sistema [OneDrive koja sadrži ispravku.](https://oneclient.sfx.ms/Mac/Prod/21.170.0822.0003/OneDrive.zip)
2. Dekomkompirujte datoteku i kopirajte OneDrive u fasciklu "Aplikacije" (tako što će zameniti postojeću OneDrive aplikaciju).

Ako treba da koristite verziju App Store, sačekajte da App Store izda verziju aplikacije koja sadrži ispravku. Nažalost, Microsoft ne može da prenese procenjeni datum izlaska fiksne verzije iz prodavnice aplikacija.


