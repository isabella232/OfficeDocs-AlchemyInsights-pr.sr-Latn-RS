---
title: Korišćenje profila e-pošte uz Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1559"
- "9000076"
ms.openlocfilehash: b1653b73e7296e7eed411ae73c19342a1187b2eb7e287cff4339ea0ca32d75c1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "53919437"
---
# <a name="using-email-profiles-with-intune"></a>Korišćenje profila e-pošte uz Intune

Intune može da se koristi za kreiranje i primenu profila e-pošte za izvorni (ugrađeni) klijent e-pošte na više platformi uređaja.

Informacije o nekim ograničenjima povezanim sa profilima e-pošte, uključujući kako se rukuje prisustvom postojećih profila i kako se uklanjaju profili e-pošte, potražite u članku Dodavanje postavki e-pošte na uređaje koji koriste [Intune.](https://docs.microsoft.com/intune/email-settings-configure)

Više informacija o kreiranju profila e-pošte za svaku platformu uređaja potražite u članku:

[Postavke Android uređaja za konfigurisanje e-pošte, potvrde identiteta i sinhronizacije u aplikaciji Intune](https://docs.microsoft.com/intune/email-settings-android)  
[Dodavanje postavki e-pošte za iOS i iPadOS uređaje u programu Microsoft Intune](https://docs.microsoft.com/intune/email-settings-ios)  
[Postavke profila e-pošte Microsoft Intune za uređaje koji rade Windows Phone 8.1](https://docs.microsoft.com/intune/email-settings-windows-phone-8-1)  
[Postavke profila e-pošte za uređaje Windows 10 u Microsoft Intune](https://docs.microsoft.com/intune/email-settings-windows-10)

**Uobičajeni problem sa sinhronizacijom**

**KNOX na Android profilu e-pošte sprečava sinhronizaciju korisničkih kontakata, kalendara i zadataka sa korisničkim uređajima.**

KNOX na Android KNOX profilu e-pošte nudi admini svom korisniku opciju da odluči koji se tipovi sadržaja sinhronizuju sa uređajem tako što će svaki od njih omogućiti.

Ako je postavka za neki od tipova sadržaja postavljena na vrednost Nije **konfigurisano** (podrazumevano), taj tip sadržaja se ne sinhronizuje automatski. Korisnik može ručno da omogući tip sadržaja koji želi, ali će ta konfiguracija biti zamenjena postavkom Intune smernica i ta sinhronizacija će prestati da se sinhronizuje za taj tip sadržaja.

