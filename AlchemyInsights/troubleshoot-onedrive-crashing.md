---
title: Rešavanje OneDrive padova
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003084"
- "5885"
ms.openlocfilehash: d5982bafbb8aaa1d240a34c071efe37e92c2ec5c5170dc59337df9a5435e22e1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "53921021"
---
# <a name="troubleshoot-onedrive-crashes"></a>Rešavanje OneDrive padova

Ako OneDrive padove, isprobajte ove korake za rešavanje problema:

**Uverite se da ključevi registratora nisu podešeni:**

1. Pomoću uređivača registratora pređite na HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive
2. Ako je postavka DisableFileSyncNGSC prisutna i postavljena na 1, otvorite ključ i promenite vrednost na 0.
3. Ručno pokretanje OneDrive tako što ćete otvoriti "Start" meni ![Pritisnite taster Windows taster](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), otkucajte OneDrive u polje za pretragu, a zatim kliknite na aplikaciju OneDrive radnoj površini.

**Uspostavite početne OneDrive:**

Napomene:

- Uspostavljanje početnih OneDrive prekida sve postojeće veze sinhronizacije (uključujući lične OneDrive ako su podešene).
- Nećete izgubiti datoteke ili podatke resetujući OneDrive na računaru.

**Da biste uspostavili OneDrive:**

1. Otvorite dijalog "Pokretanje" tako što Windows taster i taster R.
2. Ukucaj %localappdata%\Microsoft\OneDrive\onedrive.exe /reset i kliknite na dugme U redu. Komandni prozor može se pojaviti nakratko.
3. Ručno pokretanje OneDrive tako što ćete otvoriti "Start" meni ![Pritisnite taster Windows taster](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), otkucajte OneDrive u polje za pretragu, a zatim kliknite na aplikaciju OneDrive radnoj površini.

Napomene:

- Ako ste odabrali da sinhronizujete samo neke fascikle pre reset pošte, morate to da uradite ponovo kada se sinhronizacija završi. Pročitajte [izbor OneDrive fascikli za sinhronizaciju sa računarom](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)   za više informacija.
- Ovo ćete morati da dovršite za lične potrebe OneDrive i OneDrive for Business.