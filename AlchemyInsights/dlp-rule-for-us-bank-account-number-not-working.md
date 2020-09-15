---
title: DLP pravilo za broj računa u banci za sad ne radi
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
ms.openlocfilehash: eb399e4b23de32a757562833ed32d97daa6a1247
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679310"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a>DLP problemi sa brojevima američkih računa u banci

**Važno**: Tokom ovih jedinstvenih vremena, preduzimamo sve korake da bismo se uverili da će usluge SharePoint Online i OneDrive ostati dostupne u najvećoj meri – više informacija potražite u članku [Privremena prilagođavanja funkcija u usluzi SharePoint Online](https://aka.ms/ODSPAdjustments).

**DLP problemi sa brojevima američkih računa u banci**

Da li imate problema sa **prevencijom gubitka podataka (dlp)** ne radi za sadržaj koji sadrži **broj računa američkog banke** prilikom korišćenja dlp osetljive informacije u programu O365? Ako je tako, uverite se da sadržaj sadrži potrebne informacije za šta su smernice za DLP traženi prilikom procene.
  
Na primer, za polise **broja američkih računa u banci** podešene pomoću nivoa pouzdanosti 85%, sledeće se procenjuju i mora se otkriti da bi pravilo pokrenulo:
  
- **[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8-17 cifara

- **[Šara:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8-17 uzastopnih cifara.

- Provera **[zbira:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Ne, ne postoji kontrolni zbir

- **[Definicija:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** Funkcija DLP je 75% uverena da otkriva ovaj tip osetljivih informacija ako u neposrednoj blizini 300 znakova:

  - Redovni izraz Regex_usa_bank_account_number pronalazi sadržaj koji se podudara sa šarom

  - Postoji ključna reč iz Keyword_usa_Bank_Account.

    Na primer, sledeći uzorak će se pokrenuti za polise **broja američkih bankovnih računa** : proveravanje naloga 78344011

Za više informacija o tome šta je potrebno da bi se otkrio **broj broja američkog bankovnog računa** za sadržaj, pogledajte sledeći odeljak u ovom članku: [Šta osetljive informacije tipovi traže za broj američkog bankovnog računa](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number)
  
Koristite drugačiji tip pristupačnije osetljive informacije, pogledajte sledeći članak za informacije o tome šta je potrebno za druge tipove: [Šta osetljive informacije traže](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  