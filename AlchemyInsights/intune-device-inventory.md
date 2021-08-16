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
ms.openlocfilehash: 00ee4f1d7130c239272e28ee8e051a18e6e0baf13040d2a892866be5900adfaf
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "54014086"
---
# <a name="intune-device-inventory"></a>Intune zalihe uređaja

Blejd Uređaji pruža administratoru uvid u uređaje pod upravljanjem u aplikaciji Intune po uređaju. Prikazane informacije uključuju: Hardver, Otkrivene aplikacije, Stanje usaglašenosti uređaja i Stanje konfiguracije uređaja.

Podaci o zalihama za hardver i otkrivene aplikacije prikupljaju se tokom sedam dana ciklusa. Aplikacije i određeni elementi hardvera koji su prijavljeni razlikuju se u zavisnosti od operativnog sistema uređaja i toga da li je uređaj lično ili u vlasništvu preduzeća.

Više informacija potražite u [temi Pogledajte detalje o uređaju u intune.](https://docs.microsoft.com/intune/device-inventory)

**NAJČEŠĆA PITANJA**

P: Ne primam kompletnu listu aplikacija zaliha prisutnih na intune upisanim Windows uređajima. zašto da ne?

O: U ovom trenutku su samo moderne aplikacije navedene Windows 10 računara koji su identifikovani kao korporativni uređaji. Intune ne prikuplja informacije o Win32 aplikacijama instaliranim na tim uređajima.

P: Zašto se brojevi telefona ne prikupljaju sa svih uređaja?

O: Telefoni kategorizovani kao poslovni uređaji u aplikaciji Intune nisu identifikovani sa njihovim punim brojem telefona kada, na primer, pokrenete izveštaj o zalihama mobilnih uređaja. Brojevi telefona uređaja koje posedujete uvek su delimično maskirani zvezdicama (***) i prikazuju samo poslednje četiri cifre.