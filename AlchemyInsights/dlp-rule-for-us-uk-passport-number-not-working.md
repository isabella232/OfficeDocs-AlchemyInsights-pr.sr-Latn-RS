---
title: DLP pravilo za broj pasoša nam/UK ne radi
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
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: c6c7191f380f264113e2042f2869d9767922b2cc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679238"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a>Problemi sa brojevima DLP-američko/UK pasoša

**Važno**: Tokom ovih jedinstvenih vremena, preduzimamo sve korake da bismo se uverili da će usluge SharePoint Online i OneDrive ostati dostupne u najvećoj meri – više informacija potražite u članku [Privremena prilagođavanja funkcija u usluzi SharePoint Online](https://aka.ms/ODSPAdjustments).

**DP problemi sa brojevima pasoša američkih/BRITANIJA**

Da li imate problema sa **prevencijom gubitka podataka (dlp)** ne radi za sadržaj koji sadrži **broj američkog/britanskog pasoša** kada koristite Tip informacija osetljive na dlp u O365? Ako je tako, uverite se da sadržaj sadrži potrebne informacije za šta su smernice za DLP traženi prilikom procene.
  
Na primer, za smernice sa **američkom/britanski pasošem brojevima** podešene pomoću nivoa pouzdanosti 75%, sledeće se procenjuju i mora se otkriti da bi pravilo pokrenulo
  
- **[Oblikovanje:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** Devet cifara

- **[Obrazac:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** Devet uzastopnih cifara

- Provera **[zbira:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Ne, ne postoji kontrolni zbir

- **[Definicija:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** Funkcija DLP je 75% uverena da otkriva ovaj tip osetljivih informacija ako u neposrednoj blizini 300 znakova:

  - Funkcija Func_usa_uk_passport pronalazi sadržaj koji se podudara sa obrascem.

  - Postoji ključna reč iz Keyword_passport.

    Na primer, sledeći uzorak će se pokrenuti za polisu za **američke/britanski pasoš broj** : američki pasoš broj 123456789

Više informacija o tome šta je potrebno za broj za AMERIČKI/britanski pasoš da bi se otkrilo za vaš sadržaj potražite u sledećem odeljku u ovom članku: [Šta osetljive informacije tipovi traže za američki/britanski pasoš broj pasoša](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number)
  
Koristite drugačiji tip pristupačnije osetljive informacije, pogledajte sledeći članak za informacije o tome šta je potrebno za druge tipove: [Šta osetljive informacije traže](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  