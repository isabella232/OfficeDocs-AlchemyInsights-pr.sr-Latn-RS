---
title: Korišćenje profila e-pošte sa Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1559"
- "9000076"
ms.openlocfilehash: 5aae83a0ab26c2bd59fddd2ad64d1c461d29f0f7
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 07/28/2020
ms.locfileid: "46555763"
---
# <a name="using-email-profiles-with-intune"></a>Korišćenje profila e-pošte sa Intune

Intune može da se koristi za kreiranje i primenu profila e-pošte za osnovni (ugrađeni) klijent e-pošte na više platformi uređaja.

Informacije o nekim ograničenjima povezanim sa profilima e-pošte, uključujući način na koji se obrađuju prisustvo postojećih profila i kako se uklanjaju Profili e-pošte, pogledajte odeljak [Dodavanje postavki e-pošte na uređaje pomoću funkcije Intune](https://docs.microsoft.com/intune/email-settings-configure).

Više informacija o kreiranju profila e-pošte za svaku platformu uređaja potražite u članku:

[Postavke za Android uređaje da biste konfigurisali e-poštu, potvrdu identiteta i sinhronizaciju u usluzi Intune](https://docs.microsoft.com/intune/email-settings-android)  
[Dodavanje postavki e-pošte za iOS i iPadOS uređaje u programu Microsoft Intune](https://docs.microsoft.com/intune/email-settings-ios)  
[Postavke profila e-pošte u usluzi Microsoft Intune za uređaje koji rade pod operativnim sistemom Windows Phone 8,1](https://docs.microsoft.com/intune/email-settings-windows-phone-8-1)  
[Postavke profila e-pošte za uređaje koji rade pod operativnim sistemom Windows 10 u programu Microsoft Intune](https://docs.microsoft.com/intune/email-settings-windows-10)

**Uobičajeno pitanje sinhronizacije**

**KNOX na Android e-pošti profil sprečava korisničke kontakte, kalendar i zadatke, od sinhronizacije do korisničkih uređaja.**

Profil e-pošte KNOX na Android KNOX uređaju nudi administratoru opcije da odluči koji tipovi sadržaja se sinhronizuju sa uređajem tako što će podesiti svaki od njih da ih omogući.

Ako je postavka za bilo koji od tipova sadržaja postavljena na vrednost " **Nije konfigurisano** " (podrazumevani), taj tip sadržaja se neće automatski sinhronizovati. Korisnik će možda omogućiti tip sadržaja koji žele direktno na uređaj, ali ta konfiguracija se zamenjuje postavkom smernica Intune, a sinhronizacija se zaustavlja za taj tip sadržaja.

