---
title: DLP pravilo za broj kreditne kartice ne funkcioniše
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
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: bd4f200233d5571fc7b01576038e7b3951a07716a7d5948005418d2896291ee5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "54005104"
---
# <a name="dlp-issues-with-credit-card-numbers"></a>Problemi sa DLP brojevima kreditnih kartica

**Važno**: Tokom ovih jedinstvenih vremena, preduzimamo sve korake da bismo se uverili da će usluge SharePoint Online i OneDrive ostati dostupne u najvećoj meri – više informacija potražite u članku [Privremena prilagođavanja funkcija u usluzi SharePoint Online](https://aka.ms/ODSPAdjustments).

**Problemi sa DLP brojevima kreditnih kartica**

Da li imate problema sa sprečavanjem gubitka podataka **(DLP)** kada ne radite za sadržaj koji sadrži broj kreditne kartice kada koristite osetljivi tip informacija DLP u programu O365?  Ako je tako, uverite se da sadržaj sadrži potrebne informacije za aktiviranje DLP smernica kada se procene. Na primer,  za smernice kreditne kartice konfigurisane sa nivoom pouzdanosti od 85%, procenjuju se sledeće stavke i moraju se otkriti da bi pravilo trebalo da aktivira:
  
- **[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-19)** 16 cifara koje mogu da se oblikuju ili neoblikuju (ddddd) i moraju da prođu Luhn test.

- **[Obrazac:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-19)** Veoma složen i robusan obrazac koji otkriva kartice svih glavnih brendova širom sveta, uključujući Odžak, MasterCard, Otkrivanje kartice, JCB, American Express, poklon-kartice i kartice za restorane.

- **[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-19)** Da, luhn checksum

- **[Definicija:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-19)** Smernica DLP je 85% sigurni da je otkriven ovaj tip osetljivih informacija ako, u blizini od 300 znakova:

  - Funkcija Func_credit_card pronađe sadržaj koji se podudara sa obrascem.

  - Tačno je sledeće:

  - Pronađena je ključna reč Keyword_cc_verification je pronađena.

  - Pronađena je ključna Keyword_cc_name iz više reči

  - Funkcija Func_expiration_date pronađe datum u ispravnom formatu datuma.

  - Provera prolaza

    Na primer, sledeći uzorak će aktivirati smernice za broj DLP kreditne kartice:

  - Musić: 4485 3647 3952 7352
  
  - Ističe: 2.2.2009.

Dodatne informacije o tome  šta je potrebno da se otkrije broj kreditne kartice za vaš sadržaj potražite u sledećem odeljku: Šta osetljivi tipovi informacija traže za kreditnu [karticu#](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#credit-card-number)
  
Pomoću drugog ugrađenog osetljivog tipa informacija, pogledajte sledeći članak za informacije o tome šta je potrebno za druge tipove: Šta tipovi osetljivih [informacija traže](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  