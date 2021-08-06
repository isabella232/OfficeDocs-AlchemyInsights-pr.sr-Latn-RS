---
title: Pokrenite Windows dijagnostike memorije u Windows 10
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
ms.openlocfilehash: 63ba3afdd8f74b17559484f37e9250587aec9b4a929325d8f82e3c9ad06f1783
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "53922585"
---
# <a name="run-windows-memory-diagnostics-in-windows-10"></a>Pokrenite Windows dijagnostike memorije u Windows 10

Ako Windows i aplikacije na računaru padnu, zamrznu ili se ponašaju nestabilno, možda ćete naići na problem sa memorijom računara (RAM). Možete da pokrenete dijagnostiku Windows memorije da biste proverili da li ima problema sa RAM memorijom računara.

U polju za pretragu na traci zadataka otkucajte dijagnostika **memorije**, a zatim izaberite stavku Windows **memorije**. 

Da biste pokrenuli dijagnostiku, računar mora ponovo da se pokrene. Imate opciju da odmah ponovo pokrenete (sačuvajte to što ste naveli i prvo zatvorite otvorene dokumente i e-poruke) ili da zakažete da se dijagnostika pokreće automatski kada se računar sledeći put pokrene:

![Windows Dijagnostika memorije](media/windows-memory-diagnostic.png)

Kada se računar ponovo pokrene, alatka **Windows dijagnostiku** memorije će se automatski pokrenuti. Status i napredak prikazuju se dok se dijagnostika pokreće, a vi možete da otkažete dijagnostiku tako što ćete pritisnuti taster **ESC** na tastaturi.

Kada se dijagnostika završi, Windows će početi normalno.
Odmah nakon ponovnog pokretanja, kada se radna  površina pojavi, pojaviće se obaveštenje (pored ikone centra za obaveštenja na traci zadataka) koje ukazuje na to da li su pronađene bilo kakve greške u memoriji. Na primer:

Evo ikone centra aktivnosti: ![Ikona centra aktivnosti](media/action-center-icon.png) 

I probno obaveštenje: ![Nema grešaka u memoriji](media/no-memory-errors.png)

Ako ste propustili obaveštenje, možete da izaberete ikonu  centra za obaveštenja na traci zadataka da biste prikazali centar za obaveštenja i videli listu obaveštenja koja se može pomerati. 

Da biste pregledali detaljne informacije, **otkucajte događaj u** polje za pretragu na traci zadataka, a zatim izaberite **stavku Prikazivač događaja**. U **oknu "Prikazivač** događaja" sa leve strane, izaberite stavke **Windows Evidencije > Sistem**. U desnom oknu pregledajte listu dok  gledate kolonu Izvor dok ne vidite događaje sa izvornom vrednošću **MemoryDiagnostics-Results.** Istaknite svaki takav događaj i pogledajte informacije o rezultatima u okviru ispod **kartice** Opšte ispod liste.
