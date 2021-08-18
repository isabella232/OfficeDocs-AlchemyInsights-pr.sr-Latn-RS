---
title: Nadgledanje Intune uslovnog pristupa
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004636"
- "8386"
ms.openlocfilehash: 2c3a382671ac95ecbaec1b374bd8c474cf9690a2
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/13/2021
ms.locfileid: "58327571"
---
# <a name="monitor-intune-conditional-access"></a>Nadgledanje Intune uslovnog pristupa

Korisnici na koje je usmeren uslovni pristup primiće e-poruku sa obaveštenjem ako ne ispunjavaju zahteve za pristup vaše organizacije. Da biste rešili problem, preporučujemo neko od sledećih rešenja:

1. Ako se pretpostavlja da je uređaj upisan, obavestite korisnika da ode u aplikaciju Company Portal i proveri da li se uređaj pojavljuje u Company Portal. Ako nije, korisnik mora da ukuca uređaj.
1. Na Azure portalu idite na **"Usaglašenost intune**  >  **uređaja"**. 
1. Da biste prikazali izveštaj o usaglašenosti uređaja i proverili da li je uređaj korisnika označen kao usaglašen, u okviru **Nadgledanje** izaberite stavku Usaglašenost **uređaja.**
1. Na Azure portalu idite na **"Usaglašenost intune**  >  **uređaja"**. U **okviru Upravljanje izaberite** **stavku Smernice.** Na listi smernica za usaglašenost potvrdite da je profil dodeljen uređaju korisnika. Ako nije dodeljen nijedan profil, Intune neće moći da potvrdi status usaglašenosti uređaja.
1. Uredite dodelu uslovnog pristupa korisnika.
1. Na Azure portalu pređite na Stavku Smernice za uslovni pristup **intune,** izaberite smernicu sa liste, a zatim izaberite stavku Korisnici  >    >   **i grupe.**
1. Da biste određene smernice usmenili na nekoga, dodajte tu osobu **na listu Uključeno**. Da biste se uverili da je osoba izostavljana iz smernica, dodajte je na listu **Izuzeto.**

**Korisne veze:**

- [Pregled usaglašenosti uređaja](https://docs.microsoft.com/intune/device-compliance-get-started)
- [Rešavanje problema sa ca](https://docs.microsoft.com/intune/troubleshoot-conditional-access)
- [Smernice za rešavanje problema](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)
- [Nadgledanje usaglašenosti Intune uređaja](https://docs.microsoft.com/intune/compliance-policy-monitor)

**Napoome:** Ovi koraci su korisni samo za rešavanje problema Azure Active Directory funkcije "Uslovni pristup". Uređaj takođe može da karantin blokira pristup e-pošti pomoću Exchange smernica. Više informacija o Exchange upravljanju uređajima možete pronaći [**ovde.**](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141))
