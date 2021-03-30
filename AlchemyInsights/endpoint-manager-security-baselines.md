---
title: Upravljač krajnjim tačkama – osnovne linije bezbednosti
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10084"
- "6700005"
ms.openlocfilehash: d2a063fdc4929cbee5fef71bfb47ace8f2ba458f
ms.sourcegitcommit: 430d247cb5dd5dc5d1f82d977456558dfd514277
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/29/2021
ms.locfileid: "51421089"
---
# <a name="endpoint-manager---security-baselines"></a>Upravljač krajnjim tačkama – osnovne linije bezbednosti

Osnove bezbednosti su unapred konfigurisane grupe postavki operativnog sistema Windows koje vam pomažu da primenite bezbednosne postavke koje preporučuju relevantni timovi za bezbednost. Ove osnovne linije mogu da se prilagode tako da isporuče samo postavke i vrednosti koje želite. Više informacija o osnovnim linijama bezbednosti potražite u temi Korišćenje osnovnih podataka o bezbednosti za [konfigurisanje Windows 10 uređaja u aplikaciji Intune.](https://docs.microsoft.com/mem/intune/protect/security-baselines)

Trenutno postoje osnovne linije za ove proizvode:

- Windows MDM bezbednosne postavke
- Microsoft zaštitnik za bezbednost krajnje tačke
- Microsoft Edge

Svaka osnovna podataka se ažurira periodično i objavljuje u inkrementalnim verzijama. Svaka verzija dodaje ili uklanja postavke iz prethodne verzije kako bi obezbedila da osnovna linija ispunjava trenutna uputstva. Konzola osnovnih podataka bezbednosti u bezbednosti krajnje tačke omogućava poređenje različitih verzija tako što menja verzije u vidljive verzije.

Uputstva o tome kako da na najefikasnije promenite koja je verzija osnovne linije primenjena, pogledajte članak Upravljanje profilima osnovnih linija bezbednosti [u aplikaciji Microsoft Intune.](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure)

Nakon primene osnovne linije bezbednosti možete da nadgledate stanje primene i pregledate postavke na osnovu uređaja.

**Napomogućeno:** Može biti vremena da se podaci izveštavanja za osnovne podatke pojave od do 24 časa od početne primene na uređaju i do 6 časova za buduće ispravke. 

Najčešći uzrok postavke osnovne linije koja se ne primenjuje je zato što se ista postavka koristi na drugom profilu. Ovaj scenario može da se istraži za određeni uređaj tako što će izabrati taj uređaj u okviru statusa uređaja profila osnovne linije bezbednosti. Više detalja ćete videti u [temi Otklanjanje neusaglašenosti za osnovne podatke o bezbednosti.](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines)