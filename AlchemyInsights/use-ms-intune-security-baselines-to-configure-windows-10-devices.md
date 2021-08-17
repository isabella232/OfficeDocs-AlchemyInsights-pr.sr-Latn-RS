---
title: Koristite Microsoft Intune bezbednosti da biste konfigurisali Windows 10 uređaje
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
ms.openlocfilehash: a94c6b72df3874ee80413adac86d60306175734b6ff28b2e015e05eec6f3838b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "54104358"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a>Koristite Microsoft Intune bezbednosti da biste konfigurisali Windows 10 uređaje

Bezbednosne linije usluge Intune pomažu u zaštiti korisnika i uređaja. Osnove bezbednosti Windows grupe koje se koriste za primenu poznate grupe postavki i podrazumevanih vrednosti koje preporučuju relevantni timovi za bezbednost. Kreiranjem profila sa osnovnim linijama bezbednosti u programu Intune kreirate predložak koji se sastoji od više profila za konfiguraciju uređaja.

Kada primenite osnovne linije bezbednosti na grupe korisnika ili uređaja, postavke se primenjuju na uređaje koji se Windows 10 ili kasnije. Na primer, MDM bezbednosna osnovna linija automatski (1) omogućava funkciji BitLocker za prenosive disk jedinice, (2) zahteva lozinku za otključavanje uređaja, a (3) onemogućava osnovnu potvrdu identiteta. Kada podrazumevana vrednost ne funkcioniše za vaše okruženje, prilagodite osnovnu liniju da biste primenili postavke koje su vam potrebne.

Bezbednosne osnovne linije takođe pomažu u uspostavljanju sveobdnog bezbednog toka posla u Microsoft 365. Ovo su neke pogodnosti ove radnje:

- Bezbednosna osnovna linija sadrži najbolje prakse i preporuke za postavke koje utiču na bezbednost. Budući da su Intune partneri Windows timu za bezbednost koji kreira osnovne linije za smernice grupe, ove preporuke se zasnivaju na solidan vodiču i obimnom iskustvu.
- Ako ste novi korisnik usluge Intune i niste sigurni odakle da počnete, osnovne linije bezbednosti će vam pomoći da brzo napravite i primenite bezbedan profil.
- Ako trenutno koristite smernice grupe, onda je migracija u Intune u svrhe upravljanja mnogo lakša sa osnovnim linijama bezbednosti jer su ugrađene u Intune i obuhvataju vrhunske mogućnosti upravljanja.

Da biste saznali više, pogledajte [Windows osnove bezbednosti i](https://go.microsoft.com/fwlink/?linkid=2141503) Upravljanje [mobilnim uređajima.](https://go.microsoft.com/fwlink/?linkid=2141701)