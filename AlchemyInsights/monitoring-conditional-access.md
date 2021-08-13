---
title: Nadgledanje uslovnog pristupa
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9003769"
- "6702"
ms.openlocfilehash: 80e8cc72db8ae32445d48e5c8a411d5ccd538626653260b3dbd28a247561e888
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "53975115"
---
# <a name="monitoring-conditional-access-for-exchange"></a>Nadgledanje uslovnog pristupa za Exchange

Korisnici na koje je usmeren uslovni pristup primiće e-poruku sa obaveštenjem ako ne ispunjavaju zahteve za pristup vaše organizacije. Da biste rešili problem, preporučujemo neko od sledećih rešenja:

- Ako se pretpostavlja da je uređaj upisan, obavestite korisnika da ode u aplikaciju Company Portal i proveri da li se uređaj pojavljuje u Company Portal. Ako nije, korisnik bi trebalo da ukuca uređaj.
- Na Azure portalu idite na intune > usaglašenost uređaja. U okviru Nadgledanje izaberite stavku Usaglašenost uređaja. Prikažite izveštaj o usaglašenosti uređaja da biste proverili da li je uređaj korisnika označen kao usaglašen.
- Na Azure portalu idite na intune > usaglašenost uređaja. U okviru Upravljanje izaberite stavku Smernice. Na listi smernica za usaglašenost potvrdite da je profil dodeljen uređaju korisnika. Ako nije dodeljen nijedan profil, Intune neće moći da potvrdi status usaglašenosti uređaja.
- Uredite dodelu uslovnog pristupa korisnika.

1. Na Azure portalu idite na **"Smernice za intune**  >  **uslovni**  >  **pristup"**.
2. Sa liste izaberite smernicu.
3. Izaberite stavku Korisnici i grupe.
4. Da biste određene smernice usmenili na nekoga, dodajte tu osobu na listu Uključeno. Da biste se uverili da je osoba izostavljana iz smernica, dodajte je na listu Izuzeto.

Korisne veze:

[Pregled usaglašenosti uređaja](https://docs.microsoft.com/intune/device-compliance-get-started)

[Rešavanje problema sa ca](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[Smernice za rešavanje problema](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

[Nadgledanje usaglašenosti Intune uređaja](https://docs.microsoft.com/intune/compliance-policy-monitor)

Napoome: ovi koraci su korisni samo za rešavanje problema Azure Active Directory funkcije "Uslovni pristup". Uređaj takođe može da karantin blokira pristup e-pošti pomoću Exchange smernica. Više informacija o Exchange upravljanju uređajima možete pronaći [ovde]( https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141) .
