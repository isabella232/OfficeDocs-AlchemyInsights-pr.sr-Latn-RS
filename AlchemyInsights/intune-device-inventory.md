---
title: Intune zalihe uređaja
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1281"
- "6700008"
ms.openlocfilehash: 5d2be7485be8578f7fdee3216dc6f3970be67fd1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47667892"
---
# <a name="intune-device-inventory"></a>Intune zalihe uređaja

Oљtrica uređaja pruža administratorni uvid u "Uređaji" u okviru upravljanja u okviru usluge Intune na osnovu po uređaju. Prikazane informacije uključuju: hardver, pronađene aplikacije, stanje usaglašenosti uređaja i stanje konfiguracije uređaja.

Podaci o zalihama za hardver i otkrivene aplikacije se prikupljaju na sedmodnevnom ciklusu. Prijave i određeni elementi hardvera prijavljeni su u zavisnosti od operativnog sistema uređaja i da li je uređaj lično ili u vlasništvu preduzeća.

Više informacija potražite u članku [Pregled detalja uređaja u programu Intune](https://docs.microsoft.com/intune/device-inventory).

**NAJČEŠĆA PITANJA**

Q: ne primam kompletnu listu aplikacija koje su prisutne na Intune-upisanim Windows uređajima. zašto da ne?

A: sada su navedene samo moderne aplikacije za Windows 10 računare koji su identifikovani kao korporativni uređaji. Intune ne prikuplja informacije o Win32 aplikacijama instaliranih na ovim uređajima.

P: Zašto se brojevi telefona ne prikupljaju sa svih uređaja?

A: telefoni kategorizovani kao korporativni uređaji u Intune se ne identifikuju sa punim brojem telefona kada, na primer, pokrećete izveštaj o zalihama mobilnog uređaja. Broj telefonskih brojeva sa doniranim uređajima je uvek delimično maskiran sa zvezdica (* * * *) i Prikaži samo poslednje četiri cifre.