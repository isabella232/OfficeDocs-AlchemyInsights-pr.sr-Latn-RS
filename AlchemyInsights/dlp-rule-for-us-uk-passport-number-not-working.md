---
title: DLP pravilo za broj pasoša SAD/UK ne funkcioniše
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
ms.openlocfilehash: 85e3ed7fdc221981de13ab6e2ada8adf2a3a80b40ff163981e047cc4a02a1514
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "54004960"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a>Problemi sa DLP – brojevi pasoša SAD/UK

**Važno**: Tokom ovih jedinstvenih vremena, preduzimamo sve korake da bismo se uverili da će usluge SharePoint Online i OneDrive ostati dostupne u najvećoj meri – više informacija potražite u članku [Privremena prilagođavanja funkcija u usluzi SharePoint Online](https://aka.ms/ODSPAdjustments).

**Problemi sa DLP brojevima pasoša SAD/UK**

Da li imate problema sa sprečavanjem gubitka podataka **(DLP)** kada radite za sadržaj koji sadrži broj pasoša **SAD/UK** kada koristite osetljivi tip informacija u DLP-u u O365? Ako je tako, uverite se da sadržaj sadrži potrebne informacije o tome šta smernice DLP traže prilikom procene.
  
Na primer, za smernice broja pasoša **SAD/UK** konfigurisane sa nivoom pouzdanosti od 75%, procenjuju se sledeće informacije i moraju se otkriti da bi se pravilo aktiviralo
  
- **[Oblikovanje:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** Devet cifara

- **[Obrazac:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** Devet uzastopnih cifara

- **[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Ne, ne postoji provera

- **[Definicija:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** Smernica DLP je 75% sigurni da je otkriven ovaj tip osetljivih informacija ako, u blizini od 300 znakova:

  - Funkcija Func_usa_uk_passport pronađe sadržaj koji se podudara sa obrascem.

  - Pronađena je ključna reč Keyword_passport je pronađena.

    Na primer, sledeći uzorak će aktivirati smernice za broj pasoša SAD **i UK:** Broj pasoša SAD 123456789

Dodatne informacije o tome šta je potrebno da se otkrije u pasošu SAD/UK za vaš sadržaj potražite u sledećem odeljku: Šta osetljivi tipovi informacija traže za broj pasoša [SAD/UK](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number)
  
Pomoću drugog ugrađenog osetljivog tipa informacija, pogledajte sledeći članak za informacije o tome šta je potrebno za druge tipove: Šta tipovi osetljivih [informacija traže](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  