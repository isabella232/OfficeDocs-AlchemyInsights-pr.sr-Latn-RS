---
title: Saznajte ko je podesio prosleđivanje u poštanskom sandučetu i na koji način
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
ms.openlocfilehash: 6a1a1376758024339939d10a7d17520faa8505ea
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/05/2021
ms.locfileid: "50483352"
---
# <a name="find-out-who-set-up-forwarding-on-a-mailbox-and-how"></a>Saznajte ko je podesio prosleđivanje u poštanskom sandučetu i na koji način

Ako je spoljni prosleđivanje postavljen na poštansko sanduče, aktivnost se nadgleda kao deo Set-Mailbox cmdlet zapisa. Evo kako da pronađete aktivnost u evidenciji nadzora:

1. Idite na [Office 365 Security & centar za usaglašenost](https://go.microsoft.com/fwlink/p/?linkid=2077143).
1. Izaberite **stavku** >  **Pretraga evidencije nadzora**.
    > [!NOTE]
    > Ako vidite obaveštenje koje treba da uključite u nadzor, odmah ga uključite. Ako ova funkcija nije uključena, rezultati pretrage neće moći da izvuku podatke iz prethodnih datuma.
1. Proverite da li je polje **aktivnosti** podešeno da **prikazuje rezultate za sve aktivnosti** (podrazumevano). Navedite opseg datuma. Nije potrebno da navedete korisničko ime.
1. Izaberite stavku **Pretraži**. Aktivnosti se pojavljuju u okviru **Rezultati**.
1. Izaberite stavke **Filtriraj rezultate**, a zatim u polju Filter **aktivnosti** unesite **podešeno poštansko sanduče** . Ovo daje sve aktivnosti **za skupa poštanskog sandučeta** .
1. Da biste prikazali detalje, izaberite aktivnost, a zatim izaberite stavku **još informacija**. U okviru **Parametri** možete da vidite Prosleđivanje e-adrese koja je postavljena na poštansko sanduče. **ID** korisnika predstavlja korisnika koji je podesio spoljnu prosleđivanje na poštansko sanduče.
Da biste saznali više, pogledajte članak [Pretraga Office 365 evidencije nadzora radi rešavanja problema sa uobičajenim scenarijima](https://go.microsoft.com/fwlink/?linkid=2103944).