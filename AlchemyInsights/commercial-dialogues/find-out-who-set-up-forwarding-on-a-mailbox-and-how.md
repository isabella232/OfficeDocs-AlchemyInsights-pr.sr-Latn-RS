---
title: Saznajte ko je postavio prosleđivanje u poštanskom sandučetu i kako
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: 6243e787bb6b51f26cf22782d9ec80f946430b864f53de7ea626b7166a674d2c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "53988223"
---
# <a name="find-out-who-set-up-forwarding-on-a-mailbox-and-how"></a>Saznajte ko je postavio prosleđivanje u poštanskom sandučetu i kako

Ako je spoljno prosleđivanje podešeno u poštanskom sandučetu, aktivnost se nadgleda kao deo cmdlet Set-Mailbox podataka. Evo kako da pronađete aktivnost u evidenciji nadzora:

1. Idite u Office 365 [centra za & usaglašenost.](https://go.microsoft.com/fwlink/p/?linkid=2077143)
1. Izaberite **pretraga** >  **evidencije nadzora pretrage**.
    > [!NOTE]
    > Ako vidite obaveštenje da treba da uključite nadzor, uključite ga odmah. Ako ova funkcija nije uključena, rezultati pretrage neće moći da povlače podatke iz prethodnih datuma.
1. Uverite se **da je polje Aktivnosti** podešeno na Prikaži **rezultate za sve aktivnosti** (podrazumevano). Navedite opseg datuma. Ne morate da navodite korisničko ime.
1. Izaberite **stavku Pretraga**. Aktivnosti se pojavljuju u okviru **Rezultati.**
1. Izaberite **stavku Filtriranje rezultata**, a zatim **unesite podešavanje poštanskog sandučeta** u **polje filtera** Aktivnost. To daje sve aktivnosti **set-Mailbox.**
1. Da biste prikazali detalje, izaberite aktivnost, a zatim izaberite **stavku Više informacija.** U **okviru Parametri** možete da vidite adresu e-pošte za prosleđivanje koja je postavljena u poštanskom sandučetu. **UserID predstavlja** korisnika koji je postavio spoljno prosleđivanje u poštanskom sandučetu.
Da biste saznali više, pogledajte [pretragu evidencije Office 365 nadzora da biste rešili uobičajene scenarije.](https://go.microsoft.com/fwlink/?linkid=2103944)