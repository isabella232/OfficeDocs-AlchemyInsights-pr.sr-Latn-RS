---
title: Korišćenje osnovnih bezbednosnih osnovnih podataka za konfigurisanje operativnog sistema Windows 10
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/10/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8371"
- "9004622"
ms.openlocfilehash: b95454ec8ce8d0d69d1f55f7ce4adc596929e2de
ms.sourcegitcommit: 1b554c31d008492f9e6464f0249af0332212a3fc
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/10/2021
ms.locfileid: "50696380"
---
# <a name="use-the-microsoft-intune-security-baselines-for-configuring-windows-10-devices"></a>Korišćenje Microsoft Intune Security Base za konfigurisanje Windows 10 uređaja

Umetanje bezbednosnih osnovnih funkcija pomaže u zaštiti korisnika i uređaja. Osnovne bezbednosti zaštite su preliminarne grupe koje se koriste za primenu poznate grupe postavki i podrazumevanih vrednosti koje preporučuje relevantni bezbednosni timovi. Kreiranjem profila osnovne bezbednosti u Intune kreiraćete predložak koji se sastoji od profila za konfiguraciju sa više uređaja.

Kada primenite bezbednosne osnovne linije na grupe korisnika ili uređaja, postavke se primenjuju na uređaje koji se pokreću u operativnom sistemu Windows 10 ili novijim verzijama. Na primer, sigurnosna linija bezbednosti Microsoft mobilnog uređaja (MDM) automatski (1) omogućava BitLocker na prenosivim diskovima (2) zahteva lozinku za poništavanje zaključavanja uređaja i (3) onemogućava osnovnu potvrdu identiteta. Kada podrazumevana vrednost ne radi u okruženju, možete da prilagodite osnovnu liniju da biste primenili postavke koje su vam potrebne.

Osnovne bezbednosne vrednosti takođe pomažu da se uspostavi sigurnosni tok posla koji se završava u usluzi Microsoft 365. Slede neke beneficije ove funkcionalnosti:
- Osnovna osnova bezbednosti obuhvata najbolje prakse i preporuke za postavke koje utiču na bezbednost. Zato što Intune partnere sa bezbednosnim timom za Windows koji kreira osnovne linije za smernice grupe, ove preporuke su zasnovane na čvrstim vođstvima i široko iskustvo.
- Ako ste novi za podešavanje i nesigurnu odakle da počnete, osnovne bezbednosti će vam pomoći da brzo kreirate i primenite bezbedni profil.
- Ako trenutno koristite smernice grupe, a zatim Migriranje u Intune za potrebe upravljanja mnogo je lakše sa bezbednosnim osnovnim linijama, zato što su ove osnovne bezbednosti ugrađene u Intune i sadrže najsavremenije mogućnosti za upravljanje.

Više informacija potražite u članku [Windows bezbednosne osnovne linije](https://docs.microsoft.com/windows/security/threat-protection/windows-security-baselines) i [upravljanje mobilnim uređajima](https://docs.microsoft.com/windows/client-management/mdm/).