---
title: Ublažavanje greške „Ova aplikacija nije otkrivena”
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
- "9000171"
- "1712"
ms.openlocfilehash: 4e0599f9bdf2c7d16d009627f44b3691c2c250b7
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/15/2021
ms.locfileid: "51836365"
---
# <a name="mitigate-the-application-was-not-detected-error"></a>Ublažavanje greške „Ova aplikacija nije otkrivena”

Greška pri instalaciji aplikacije, „Aplikacija nije otkrivena nakon uspešnog završetka instalacije”, koju prijavljuje Intune, može da se pojavi na svim većim OS platformama (Windows, iOS i Android).

Najčešći scenariji koji generišu ovu grešku uključuju:

- Aplikacija je ažurirana izvan same Intune aplikacije (iz prodavnice nezavisnih proizvođača) posle početne primene. Na primer, neke aplikacije kao što je Google Chrome mogu da izvrše automatsko ažuriranje.
- Korisnik je deinstalirao aplikaciju nakon početne instalacije.

Da biste ublažili ovaj problem, prvo izvršite pregled pogođenih uređaja da biste odredili scenario u kom se greška događa.

- Ako je aplikacija ažurirana izvan same Intune aplikacije, primena aplikacije može se podesiti tako da zanemari verziju aplikacije. Da biste to uradili, u okviru **Konfiguracije aplikacije > Informacije o aplikaciji**, postavite **Zanemari verziju aplikacije** na **Da**.
- Kada ciljate klijenta, možda bi trebalo da primenite aplikaciju kao „obaveznu” i da osigurate da je primenjena najnovija verzija.
- Druga mogućnost je da na iOS platformi možete da koristite funkcionalnost **automatskog ažuriranja** koja je povezana sa programom za količinsku kupovinu kompanije Apple, koji se može konfigurisati tako da automatski ažurira aplikacije kada nove verzije postanu dostupne.

Dodatne informacije o rešavanju problema sa instalacijom aplikacija potražite u članku [Rešavanje problema prilikom instalacije aplikacije](https://docs.microsoft.com/intune/troubleshoot-app-install).
