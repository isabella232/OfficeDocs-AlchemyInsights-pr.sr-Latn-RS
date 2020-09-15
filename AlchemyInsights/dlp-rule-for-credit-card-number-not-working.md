---
title: DLP pravilo za broj kreditne kartice ne radi
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
ms.openlocfilehash: d5dd6354e7a1bcbb7f2fb917952ddbee5077e88d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679455"
---
# <a name="dlp-issues-with-credit-card-numbers"></a>DLP problemi sa brojevima kreditnih kartica

**Važno**: Tokom ovih jedinstvenih vremena, preduzimamo sve korake da bismo se uverili da će usluge SharePoint Online i OneDrive ostati dostupne u najvećoj meri – više informacija potražite u članku [Privremena prilagođavanja funkcija u usluzi SharePoint Online](https://aka.ms/ODSPAdjustments).

**DLP problemi sa brojevima kreditnih kartica**

Da li imate problema sa **prevencijom gubitka podataka (dlp)** ne radi za sadržaj koji sadrži **broj kreditne kartice** prilikom korišćenja tipa dlp osetljive informacije u programu O365? Ako je tako, uverite se da sadržaj sadrži potrebne informacije za pokretanje DLP smernica kada se proceni. Na primer, za **smernice kreditne kartice** podešene pomoću nivoa pouzdanosti 85%, sledeće se procenjuju i mora se otkriti da bi pravilo pokrenulo:
  
- **[Oblikovanje:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-19)** 16 cifara koje mogu da se oblikuju ili neoblikovane (dddddddddddddddd) i moraju da proslede luhn test.

- **[Obrazac:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-19)** Veoma složen i robusan šara koji prepoznaje kartice svih velikih brendova širom sveta, uključujući vizu, MasterCard, karticu otkrivanja, JCB, American Express, poklon-razglednice i иestitke za restoran.

- Provera **[zbira:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-19)** Da, polje "Luhn"

- **[Definicija:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-19)** Funkcija DLP je 85% uverena da otkriva ovaj tip osetljivih informacija ako u neposrednoj blizini 300 znakova:

  - Funkcija Func_credit_card pronalazi sadržaj koji se podudara sa obrascem.

  - Tačno:

  - Postoji ključna reč iz Keyword_cc_verification.

  - Pronađena je ključna reč iz Keyword_cc_name

  - Funkcija Func_expiration_date pronalazi datum u pravom formatu za datum.

  - Propusnice za proveru

    Na primer, sledeći uzorak će se pokrenuti radi smernica za DEP kreditnu karticu:

  - Viza: 4485 3647 3952 7352
  
  - Ističe: 2/2009

Više informacija o tome šta je potrebno da bi se video **broj kreditne kartice** detektovano za sadržaj potražite u sledećem odeljku u ovom članku: [koje vrste osetljivim informacija traže kreditnu karticu "](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#credit-card-number)
  
Koristite drugačiji tip pristupačnije osetljive informacije, pogledajte sledeći članak za informacije o tome šta je potrebno za druge tipove: [Šta osetljive informacije traže](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  