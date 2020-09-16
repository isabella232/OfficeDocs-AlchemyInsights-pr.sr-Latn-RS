---
title: Korišćenje profila e-pošte sa Intune
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
ms.openlocfilehash: 92d91de5d369eb9d0ffde2580b75376035a6945b
ms.sourcegitcommit: 483444ab35ab0e4d410d121562045efde47aa61a
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47653302"
---
# <a name="using-email-profiles-with-intune"></a>Korišćenje profila e-pošte sa Intune

Intune se mogu koristiti za kreiranje i primenu profila e-pošte za poreklom (ugrađeni) klijent e-pošte na više platformi uređaja.

Informacije o nekom od ograničenja koja se odnose na profile e-pošte, uključujući kako se rukuje prisutnost postojećeg profila i kako da uklonite profile e-pošte, potražite [u članku Dodavanje postavki e-pošte u uređaje pomoću Intune](https://docs.microsoft.com/intune/email-settings-configure).

Više informacija o tome kako da kreirate profile e-pošte za svaku platformu uređaja potražite u članku:

[Postavke Android uređaja da biste konfigurisali e-poštu, potvrdu identiteta i sinhronizaciju u Intune](https://docs.microsoft.com/intune/email-settings-android)  
[Dodavanje postavki e-pošte za iOS i iPadOS uređaje u usluzi Microsoft Intune](https://docs.microsoft.com/intune/email-settings-ios)  
[Postavke profila e-pošte u programu Microsoft Intune za uređaje koje koriste Windows Phone 8,1](https://docs.microsoft.com/intune/email-settings-windows-phone-8-1)  
[Postavke profila e-pošte za uređaje koji rade pod operativnim sistemom Windows 10 u programu Microsoft Intune](https://docs.microsoft.com/intune/email-settings-windows-10)

**Uobičajeni problem sa sinhronizacijom**

**KNOX na Android profilu e-pošte sprečava korisnike, kalendar i zadatke da se sinhronizuju sa korisničkim uređajima.**

Profil e-pošte na Android KNOX-u pruža programu administrator opciju da odluči koji tipovi sadržaja se sinhronizuju sa uređajem tako što će se podesiti svako omogućen.

Ako je postavka za bilo koji tip sadržaja podešena tako da **ne bude podešena** (podrazumevano), taj tip sadržaja se ne sinhronizuje automatski. Korisnik može da omogući ručno željeni tip sadržaja, ali ta konfiguracija se zamenjuje pomoću postavke Intune, a sinhronizacija prestaje za taj tip sadržaja.

