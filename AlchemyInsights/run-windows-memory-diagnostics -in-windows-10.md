---
title: Pokretanje Windows dijagnostike memorije u operativnom sistemu Windows 10
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002959"
- "5661"
ms.openlocfilehash: ff8f80b3df4e3809e844195128f4d99cbc4667be
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826681"
---
# <a name="run-windows-memory-diagnostics-in-windows-10"></a>Pokretanje Windows dijagnostike memorije u operativnom sistemu Windows 10

Ako Windows i aplikacije na računaru padnu, zamrznu se ili se ponašaju nestabilno, možda ćete naići na problem sa memorijom računara (RAM). Možete da pokrenete Windows dijagnostiku memorije da biste proverili da li ima problema sa RAM memorijom računara.

U polje za pretragu na traci zadataka ukucajte **dijagnostika memorije**, a zatim izaberite **stavku Windows dijagnostika memorije**. 

Da biste pokrenuli dijagnostiku, računar mora ponovo da se pokrene. Imate opciju da odmah ponovo pokrenete (sačuvajte to što ste naveli i prvo zatvorite otvorene dokumente i e-poruke) ili da zakažete da se dijagnostika pokreće automatski kada se računar sledeći put pokrene:

![Windows dijagnostika memorije](media/windows-memory-diagnostic.png)

Kada se računar ponovo pokrene, Windows alatka za **dijagnostiku memorije** će se automatski pokrenuti. Status i napredak prikazuju se dok se dijagnostika pokreće, a vi možete da otkažete dijagnostiku tako što ćete pritisnuti taster **ESC** na tastaturi.

Kada se dijagnostika završi, Windows će početi normalno.
Odmah nakon ponovnog pokretanja, kada se radna  površina pojavi, pojaviće se obaveštenje (pored ikone centra za obaveštenja na traci zadataka) koje ukazuje na to da li su pronađene bilo kakve greške u memoriji. Na primer:

Evo ikone centra aktivnosti: ![Ikona centra aktivnosti](media/action-center-icon.png) 

I probno obaveštenje: ![Nema grešaka u memoriji](media/no-memory-errors.png)

Ako ste propustili obaveštenje, možete da izaberete ikonu  centra za obaveštenja na traci zadataka da biste prikazali centar za obaveštenja i videli listu obaveštenja koja se može pomerati. 

Da biste pregledali detaljne informacije, **otkucajte događaj u** polje za pretragu na traci zadataka, a zatim izaberite **stavku Prikazivač događaja**. U **oknu "Prikazivač** događaja" sa leve strane, izaberite stavke **Windows evidencije > Sistem**. U desnom oknu pregledajte listu dok  gledate kolonu Izvor dok ne vidite događaje sa izvornom vrednošću **MemoryDiagnostics-Results.** Istaknite svaki takav događaj i pogledajte informacije o rezultatima u okviru ispod **kartice** Opšte ispod liste.
