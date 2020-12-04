---
title: Korišćenje Microsoft Intune Base Security za konfigurisanje Windows 10 uređaja
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004135"
- "7211"
ms.openlocfilehash: 24257f1ac5752df1598d08fcfdb95ee2642adfea
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573532"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a>Korišćenje Microsoft Intune Base Security za konfigurisanje Windows 10 uređaja

Umetanje bezbednosnih osnovnih funkcija pomaže u zaštiti korisnika i uređaja. Osnovne bezbednosti zaštite su preliminarne grupe koje se koriste za primenu poznate grupe postavki i podrazumevanih vrednosti koje preporučuje relevantni bezbednosni timovi. Kreiranjem profila osnovne bezbednosti u Intune kreiraćete predložak koji se sastoji od profila za konfiguraciju sa više uređaja.

Kada primenite bezbednosne osnovne linije na grupe korisnika ili uređaja, postavke se primenjuju na uređaje koji se pokreću u operativnom sistemu Windows 10 ili novijim verzijama. Na primer, komanda "MDM Security" automatski (1) omogućava BitLocker za prenosive diskove, (2) zahteva lozinku za poništavanje zaključavanja uređaja i (3) onemogućava osnovnu potvrdu identiteta. Kada podrazumevana vrednost ne radi u okruženju, prilagodite osnovnu liniju da biste primenili postavke koje su vam potrebne.

Osnovne bezbednosne vrednosti takođe pomažu da se uspostavi sigurnosni tok posla koji se završava u usluzi Microsoft 365. Slede neke beneficije:

- Osnovna osnova bezbednosti obuhvata najbolje prakse i preporuke za postavke koje utiču na bezbednost. Zato što Intune partnere sa bezbednosnim timom za Windows koji kreira osnovne linije za smernice grupe, ove preporuke su zasnovane na čvrstim vođstvima i široko iskustvo.
- Ako ste novi za podešavanje i nesigurnu odakle da počnete, osnovne bezbednosti će vam pomoći da brzo kreirate i primenite bezbedni profil.
- Ako trenutno koristite smernice grupe, a zatim Migriranje u Intune za potrebe upravljanja mnogo je lakše sa bezbednosnim osnovnim linijama, zato što su ugrađene u Intune i sadrže najsavremenije mogućnosti za upravljanje.

Da biste saznali više, pogledajte članak [Windows Security osnovni](https://go.microsoft.com/fwlink/?linkid=2141503) [Uređaji i upravljanje mobilnim uređajima](https://go.microsoft.com/fwlink/?linkid=2141701).