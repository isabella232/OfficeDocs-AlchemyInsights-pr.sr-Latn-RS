---
title: Rešavanje problema sa OneDrive padovima
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003084"
- "5885"
ms.openlocfilehash: 1155d370911b28bbb1ba83a15eace66d1daea28f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47665012"
---
# <a name="troubleshoot-onedrive-crashes"></a>Rešavanje problema sa OneDrive padovima

Ako OneDrive više puta pada, isprobajte ove korake za rešavanje problema:

**Obezbedite da nisu podešeni ključevi registratora:**

1. Korišćenje uređivača registratora potražite u HKEY_LOCAL_MACHINE \SOFTWARE\Policies\Microsoft\OneDrive
2. Ako je funkcija Oneblefilesyncngsc postavljena na 1, otvorite ključ i promenite vrednost u 0.
3. Ručno pokretanje usluge OneDrive tako što ćete početi ![Pritisnite taster Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), u polju za pretragu otkucajte OneDrive, a zatim kliknite na OneDrive aplikaciju za računare.

**Poništavanje OneDrive:**

Primeć

- Ponovno podešavanje usluge OneDrive prekida sve postojeće veze sinhronizacije (uključujući lični OneDrive ako je podešeno).
- Nećete izgubiti datoteke ili podatke tako što ćete ponovo postaviti OneDrive na računaru.

**Da biste poništili OneDrive:**

1. Otvorite dijalog "pokreće" tako što ćete pritisnuti taster Windows Key i R.
2. Otkucajte% LocalAppData% \Microsoft\OneDrive\onedrive.exe/reset i pritisnite u redu. Prozor sa komandama može da se pojavi nakratko.
3. Ručno pokretanje usluge OneDrive tako što ćete početi ![Pritisnite taster Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), u polju za pretragu otkucajte OneDrive, a zatim kliknite na OneDrive aplikaciju za računare.

Primeć

- Ako ste odabrali da sinhronizujete samo neke fascikle pre ponovnog početnih vrednosti, moraćete to ponovo da uradite kada se sinhronizacija dovrši. Pročitajte [stavku Odaberite koje OneDrive fascikle želite da sinhronizujete sa računarom](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)   za više informacija.
- Moraćete da dovršite ovo za ličnu OneDrive i OneDrive for Business.