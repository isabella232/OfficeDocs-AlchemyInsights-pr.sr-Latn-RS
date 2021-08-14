---
title: DLP pravilo za broj bankovnog računa u SAD ne funkcioniše
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
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: d19b2dcc29e23fab522159945496165338a117a47bfcfcadf0b93e4e5f14464f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "54005032"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a>Problemi sa DLP-om sa brojevima bankovnih računa u SAD

**Važno**: Tokom ovih jedinstvenih vremena, preduzimamo sve korake da bismo se uverili da će usluge SharePoint Online i OneDrive ostati dostupne u najvećoj meri – više informacija potražite u članku [Privremena prilagođavanja funkcija u usluzi SharePoint Online](https://aka.ms/ODSPAdjustments).

**Problemi sa DLP-om sa brojevima bankovnih računa u SAD**

Da li imate problema sa sprečavanjem gubitka podataka **(DLP)** prilikom korišćenja osetljivog tipa informacija u DLP-u  u O365? Ako je tako, uverite se da sadržaj sadrži potrebne informacije o tome šta smernice DLP traže prilikom procene.
  
Na primer, za smernice broja bankovnog računa u **SAD** konfigurisane sa nivoom pouzdanosti od 85%, procenjuju se sledeće stavke i moraju se otkriti da bi se pravilo aktiviralo:
  
- **[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8–17 cifara

- **[Obrazac:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8–17 uzastopnih cifara.

- **[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Ne, ne postoji provera

- **[Definicija:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** Smernica DLP je 75% sigurni da je otkriven ovaj tip osetljivih informacija ako, u blizini od 300 znakova:

  - Običan izraz Regex_usa_bank_account_number pronađe sadržaj koji se podudara sa obrascem

  - Pronalaže se ključna Keyword_usa_Bank_Account iz e-Keyword_usa_Bank_Account.

    Na primer, sledeći uzorak će aktivirati smernice za broj bankovnog računa u **SAD:** provera broja 78344011

Dodatne informacije o tome šta je potrebno da se otkrije broj bankovnog računa u **SAD** za sadržaj potražite u sledećem odeljku u ovom članku: Šta osetljivi tipovi informacija traže za broj bankovnog računa u [SAD](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number)
  
Pomoću drugog ugrađenog osetljivog tipa informacija, pogledajte sledeći članak za informacije o tome šta je potrebno za druge tipove: Šta tipovi osetljivih [informacija traže](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  