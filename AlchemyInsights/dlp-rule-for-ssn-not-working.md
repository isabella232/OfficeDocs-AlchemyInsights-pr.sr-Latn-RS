---
title: DLP pravilo za SSN ne funkcioniše
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
ms.openlocfilehash: 3f30998fb3bc4c5442e4e1541b87d88ecd7df6eef3a50e719fa5014eb86af39c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "54004996"
---
# <a name="dlp-issues-with-social-security-numbers"></a>DLP problemi sa društvenim bezbednosnim brojevima

**Važno**: Tokom ovih jedinstvenih vremena, preduzimamo sve korake da bismo se uverili da će usluge SharePoint Online i OneDrive ostati dostupne u najvećoj meri – više informacija potražite u članku [Privremena prilagođavanja funkcija u usluzi SharePoint Online](https://aka.ms/ODSPAdjustments).

**Problemi sa DLP-om sa SSN-ovima**

Da li imate problema sa sprečavanjem gubitka podataka **(DLP)** prilikom korišćenja osetljivog tipa informacija u programu Microsoft 365?  Ako je tako, uverite se da sadržaj sadrži potrebne informacije za ono što DLP smernice traže. 
  
Na primer, za SSN smernice konfigurisane sa nivoom pouzdanosti od 85%, procenjuju se sledeće stavke i moraju se otkriti da bi se pravilo aktiviralo:
  
- **[Format:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 cifara, koje mogu biti oblikovane ili neoblikirane šare

- **[Obrazac:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Četiri funkcije traže SSN-ove u četiri različita obrasca:

  - Func_ssn SSN-ove sa jakim oblikovanjem pre 2011. koje je oblikovano u isecima ili razmacima (ddd-dddd OR ddd dddd dd)

  - Func_unformatted_ssn SSN-a sa unapred iz 2011. jakom oblikovanjem koje nije oblikovano kao devet uzastopnih cifara (dddddddd)

  - Func_randomized_formatted_ssn SSN-2011 koji su oblikovani sa isecima ili razmacima (ddd-dddd OR ddd dddd OR dd)

  - Func_randomized_unformatted_ssn SSN-2011. koji nisu oblikovani kao devet uzastopnih cifara (dddddddd)

- **[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** Ne, ne postoji provera

- **[Definicija:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** Smernica DLP je 85% sigurni da je otkriven ovaj tip osetljivih informacija ako, u blizini od 300 znakova:

  - Funkcija [Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) pronađe sadržaj koji se podudara sa obrascem.

  - Pronađena je ključna [reč Keyword_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn) je pronađena. Primeri ključnih reči su:  *Social Security, Social Security#, Soc Sec ,SSN*  . Na primer, sledeći uzorak će aktivirati DLP SSN **smernice: SSN: 489-36-8350**
  
Više informacija o tome šta je potrebno da SSN-ove otkriju za sadržaj potražite u sledećem odeljku u ovom članku: Šta osetljivi tipovi informacija traže za [SSN-ove](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn)
  
Pomoću drugog ugrađenog osetljivog tipa informacija, pogledajte sledeći članak za informacije o tome šta je potrebno za druge tipove: Šta tipovi osetljivih [informacija traže](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  