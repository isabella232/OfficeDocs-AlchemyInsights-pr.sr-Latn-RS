---
title: DLP pravilo za SSN ne radi
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
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: b221e66862ca01074f380fbb8433f8f9cac044cb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679383"
---
# <a name="dlp-issues-with-social-security-numbers"></a>DLP problemi sa brojevima socijalnog osiguranja

**Važno**: Tokom ovih jedinstvenih vremena, preduzimamo sve korake da bismo se uverili da će usluge SharePoint Online i OneDrive ostati dostupne u najvećoj meri – više informacija potražite u članku [Privremena prilagođavanja funkcija u usluzi SharePoint Online](https://aka.ms/ODSPAdjustments).

**LINP problemi sa SNS-ovima**

Da li imate problema sa **prevencijom gubitka podataka (DLP)** ne radi za sadržaj koji sadrži **broj socijalnog osiguranja (SSN)** kada koristite osetljiv tip informacija u usluzi Microsoft 365? Ako je tako, uverite se da sadržaj sadrži potrebne informacije za ono što traži DLP smernice. 
  
Na primer, za SSN smernice podešene pomoću nivoa pouzdanosti 85%, sledeće se procenjuju i mora se otkriti da bi pravilo pokrenulo:
  
- **[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 cifara, što je možda u oblikovanom ili neoblikovanom obrascu

- **[Obrazac:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Četiri funkcije traže SSNs u četiri različita šablona:

  - Func_ssn pronalazi SSNs sa jakim oblikovanjem pre 2011 koje su oblikovane pomoću crtica ili razmaka (DDD-dd-dddd ili DDD dd dddd)

  - Func_unformatted_ssn pronalazi Ssnsa sa jakim oblikovanjem pre 2011 koje su neoblikovane kao devet uzastopnih cifara (ddddddddddd)

  - Func_randomized_formatted_ssn pronalazi 2011 SSNs koji su oblikovani sa crtama ili razmacima (DDD-dd-dddd ili DDD dd dddd)

  - Func_randomized_unformatted_ssn pronalazi 2011 SSNs koje nisu oblikovane kao devet uzastopnih cifara (ddddddddd)

- Provera **[zbira:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** Ne, ne postoji kontrolni zbir

- **[Definicija:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** Funkcija DLP je 85% uverena da otkriva ovaj tip osetljivih informacija ako u neposrednoj blizini 300 znakova:

  - [Funkcija Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) pronalazi sadržaj koji se podudara sa obrascem.

  - Postoji ključna reč iz [Keyword_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn) . Primeri ključnih reči uključuju:  *socijalnu bezbednost, socijalnu bezbednost #, soc sec, SSN*  . Na primer, sledeći uzorak će se pokrenuti za DP SSN smernice: **SSN: 489-36-8350**
  
Za više informacija o tome šta je potrebno da bi se Snsa otkrilo za vaš sadržaj, pogledajte sledeći odeljak u ovom članku: [Šta osetljive informacije tipovi traže za SSNs](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn)
  
Koristite drugačiji tip pristupačnije osetljive informacije, pogledajte sledeći članak za informacije o tome šta je potrebno za druge tipove: [Šta osetljive informacije traže](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  