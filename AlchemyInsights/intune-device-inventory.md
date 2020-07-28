---
title: Intune na zalihama uređaja
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1281"
- "6700008"
ms.openlocfilehash: d59ee014a64de39d01837e90909619f30ec35e89
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 07/28/2020
ms.locfileid: "45440475"
---
# <a name="intune-device-inventory"></a>Intune na zalihama uređaja

Uređaj Blade obezbeđuje administratorsku uvid u uređaje pod upravom u usluzi Intune na osnovu uređaja. Prikazane informacije uključuju: hardver, otkrivene aplikacije, stanje usaglašenosti uređaja i stanje konfiguracije uređaja.

Podaci o zalihama za hardverske i otkrivene aplikacije prikupljaju se u sedmodnevnom ciklusu. Aplikacije i specifični elementi hardvera su se razlikovale u zavisnosti od operativnog sistema uređaja, kao i od toga da li je uređaj lično ili u vlasništvu preduzeća.

Za više informacija pogledajte odeljak [pregled informacija o uređaju u usluzi Intune](https://docs.microsoft.com/intune/device-inventory).

**NAJČEŠĆA PITANJA**

Q: Neću primati popis aplikacija prisutnih na Intune-upisan Windows uređaje. Zašto da ne?

A: u ovom trenutku su samo moderne aplikacije navedene za Windows 10 računare koji su identifikovani kao korporativni uređaji. Intune ne prikuplja informacije o Win32 aplikacijama instaliranim na ovim uređajima.

Q: Zašto se brojevi telefona ne prikupljaju sa svih uređaja?

A: telefoni kategorizovani kao korporativni uređaji u Intune nisu identifikovani sa punim telefonskim brojem kada, na primer, pokrećete izveštaj o zalihama za mobilni uređaj. Brojevi telefona na vašem uređaju su uvek delimično maskirani sa zvezdicom (* * * *) i prikazuju samo poslednje četiri cifre.