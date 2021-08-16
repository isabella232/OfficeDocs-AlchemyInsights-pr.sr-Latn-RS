---
title: Izvoz e-discovery/Content Search rezultata
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
- "3200003"
- "7221"
ms.openlocfilehash: de5d6f2bbf32ca1b7a0bbb9dd416fb19186d2e72ad57fbf25d9b55bd733fdc21
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "53988140"
---
# <a name="export-ediscoverycontent-search-results"></a>Izvoz e-discovery/Content Search rezultata

Možda ćete morati da izvezete rezultate pretrage u PST datoteku (iz e-pošte) ili u Kancelarija dokumente (sa lokacija SharePoint i OneDrive for Business sajtova). Ako je to moguće, uradite sledeće:

- Uverite se da su nalogu dodeljene odgovarajuće dozvole za izvoz. Dodatne informacije potražite u [članku Dodela dozvole za e-discovery](https://go.microsoft.com/fwlink/?linkid=2102406).
- Uverite se da računar ispuni [sve preduslove](https://docs.microsoft.com/office365/securitycompliance/export-search-results#before-you-begin). Nisu podržani svi pregledači, kao što je Chrome.
- Da biste izvezli iz pretrage sadržaja: a. Idite u centar za & [usaglašenosti i kliknite](https://protection.office.com/contentsearch) na dugme **Pretraga**, a zatim **izaberite stavku Pretraga sadržaja.** Na stranici **Pretraga sadržaja** izaberite sačuvanu pretragu.
    b. U oknu Detalji, u okviru **Izvoz rezultata na računar izaberite** stavku Pokreni **izvoz**. Ako izvozite više od 100K poštannih sandučića, biće potrebno da koristite PowerShell da biste preuzeli rezultate izvoza. Dodatne informacije potražite u [članku Izvoz rezultata iz više od 100K poštannih sandučića.](https://go.microsoft.com/fwlink/?linkid=2143861)

Da biste saznali više, pogledajte izvoz [rezultata pretrage sadržaja.](https://go.microsoft.com/fwlink/?linkid=2102118)