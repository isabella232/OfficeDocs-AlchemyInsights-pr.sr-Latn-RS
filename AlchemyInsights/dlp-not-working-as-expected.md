---
title: DLP ne radi na očekivani način
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: 0ed893420b5813d5d18639c2c226c12f0306a13f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679707"
---
# <a name="dlp-not-working-as-expected"></a>DLP ne radi na očekivani način

**Važno**: Tokom ovih jedinstvenih vremena, preduzimamo sve korake da bismo se uverili da će usluge SharePoint Online i OneDrive ostati dostupne u najvećoj meri – više informacija potražite u članku [Privremena prilagođavanja funkcija u usluzi SharePoint Online](https://aka.ms/ODSPAdjustments).

 **Podešavanje DLP**

Da li imate problema sa **prevencijom gubitka podataka (DLP)** u sistemu Office 365 ne radite kao što je očekivano? Ako je tako, proverite da li su **smernice za dlp** ispravno podešene i da vaši podaci sadrže ono što traži **dlp smernice** kada se procenjuje.
  
DLP smernice vam omogućavaju da identifikujete i zaštitite osetljive informacije u organizaciji. Da biste postavili programe DLP, koristite ove informacije [ovde](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).
  
 **Koje programe za DLP traže**
  
Kada koristite **ugrađene osetljive tipove informacija** u centrima bezbednosti i usaglašenosti, dlp smernice traže specifične obrasce i elemente prilikom detekcija ovih osetljivih tipova.
  
- **Ugrađeni osetljivi tipovi informacija**

    Informacije o ugrađenim osetljivim tipovima i tome koje smernice za DLP traže kada otkrivaju osetljiv tip, pogledajte članak: [Šta osetljive informacije traže](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).

- **Tipovi prilagođenih informacija**

    Ako pokušavate da kreirate prilagođene osetljive informacije, koristite sledeći članak za informacije o tome kako da kreirate prilagođeni osetljivi tip [informacija: Kreirajte tip prilagođene osetljive informacije](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type).

**Testiranje DP smernica**

Da biste testirali podatke sa ugrađenim ili prilagođene osetljive informacije, koristite opciju **tip testa** u okviru **klasifikacija**  >  **osetljivih informacija**. Više informacija potražite u članku [testiranje tipova prilagođenih osetljivih informacija](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center).

 **O**
  
- Nabavite osetljive informacije [o Dlp izveštajima.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)

- Pogledajte određene detalje događaja sa [izveštajem o incidentu](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports).
