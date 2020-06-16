---
title: Rešavanje problema sa OneDrive padovima
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003084"
- "5885"
ms.openlocfilehash: 7fbc4617a0426eb11359339edc950a108f782750
ms.sourcegitcommit: 462522e6bccde76f6c46795b0eca71320c5d442d
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 06/15/2020
ms.locfileid: "44749167"
---
# <a name="troubleshoot-onedrive-crashes"></a>Rešavanje problema sa OneDrive padovima

Ako OneDrive više puta padne, isprobajte ove korake za rešavanje problema:

**Uverite se da ključevi registratora nisu podešeni:**

1. Pomoću programa Registry Editor Krećite se do HKEY_LOCAL_MACHINE \SOFTWARE\Policies\Microsoft\OneDrive
2. Ako je DisableFileSyncNGSC prisutan i postavljen na 1, otvorite ključ i promenite vrednost u 0.
3. Ručno pokretanje usluge OneDrive tako što ćete otići na početni ekran ![Pritisnite taster sa Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)Otkucajte OneDrive u polju za pretragu, a zatim kliknite na aplikaciju OneDrive radne površine.

**Poništi OneDrive:**

Beleške:

- Uspostavljanje početnih vrednosti usluge OneDrive prekida vezu sa svim postojećim sinhronizovanim vezama (uključujući i vašu ličnu OneDrive ako je podešeno).
- Datoteke ili podatke nećete izgubiti tako što ćete ponovo da pokrenete OneDrive na računaru.

**Da biste uspostavili početne vrednosti usluge OneDrive:**

1. Otvorite dijalog "pokretanje" tako što ćete pritisnuti Windows taster i R.
2. Otkucajte% LocalAppData% \Microsoft\OneDrive\onedrive.exe/reset i Pritisnite OK. Moguće je da će komandni prozor biti nakratko prikazan.
3. Ručno pokretanje usluge OneDrive tako što ćete otići na početni ekran ![Pritisnite taster sa Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)Otkucajte OneDrive u polju za pretragu, a zatim kliknite na aplikaciju OneDrive radne površine.

Beleške:

- Ako ste odabrali da sinhronizujete samo neke fascikle pre nego što uspostavite početne vrednosti, biće potrebno da to uradite ponovo kada se sinhronizacija dovrši. Pročitajte [izbor koje OneDrive fascikle želite da sinhronizujete sa računarom](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)da biste   dobili više informacija.
- Ovo ćete morati da dovršite za vaše lične usluge OneDrive i OneDrive za posao.