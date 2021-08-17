---
title: Korišćenje Microsoft Intune bezbednosti osnovnih podataka za konfigurisanje Windows 10 uređaja
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9006500"
- "11142"
ms.openlocfilehash: f77fdbb315db8317a6a1374f05489a7f5a0bedcec484dc9ac53a473098583949
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/11/2021
ms.locfileid: "57886646"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a>Korišćenje Microsoft Intune bezbednosti osnovnih podataka za konfigurisanje Windows 10 uređaja

Bezbednosne linije usluge Intune pomažu u zaštiti korisnika i uređaja. Osnove bezbednosti su Windows postavke koje su unapred konfigurisane za primenu poznate grupe postavki i podrazumevanih vrednosti koje preporučuju relevantni timovi za bezbednost. Kreiranjem profila sa osnovnim linijama bezbednosti u programu Intune kreirate predložak koji se sastoji od više profila za konfiguraciju uređaja.

Kada primenite osnovne linije bezbednosti na grupe korisnika ili uređaja, postavke se primenjuju na uređaje koji se Windows 10 ili kasnije. Na primer, bezbednosna linija za upravljanje Microsoft mobilnim uređajima (MDM) automatski omogućava BitLocker za prenosive disk jedinice, zahteva lozinku za otključavanje uređaja i onemogućava osnovnu potvrdu identiteta. Kada podrazumevana vrednost ne funkcioniše za okruženje, možete da prilagodite osnovnu liniju da biste primenili postavke koje su vam potrebne.

Bezbednosne osnovne linije takođe pomažu u uspostavljanju sveobdnog bezbednog toka posla u Microsoft 365. Bezbednosna osnovna linija sadrži najbolje prakse i preporuke za postavke koje utiču na bezbednost. Intune partneri sa Windows za bezbednost koji pravi osnovne linije za smernice grupe, tako da se ove preporuke zasnivaju na solid smernicama i obimnom iskustvu.

Ako ste novi korisnik usluge Intune i niste sigurni odakle da počnete, osnovne linije bezbednosti vam pomažu da brzo napravite i primenite bezbedan profil. Ako trenutno koristite smernice grupe, migracija u Intune u svrhe upravljanja mnogo je lakša sa osnovnim linijama bezbednosti jer su ugrađene u intune i obuhvataju mogućnosti upravljanja isecanjem ivica.

Da biste saznali više, pogledajte [Windows osnove bezbednosti](https://docs.microsoft.com/windows/security/threat-protection/windows-security-baselines) i Upravljanje [mobilnim uređajima.](https://docs.microsoft.com/windows/client-management/mdm/)

