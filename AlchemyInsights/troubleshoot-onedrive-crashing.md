---
title: Rešavanje problema sa padima u usluzi OneDrive
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
ms.openlocfilehash: 4bf45e7780dcbabb95b3eecfb2df55beffde11d6
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826213"
---
# <a name="troubleshoot-onedrive-crashes"></a>Rešavanje problema sa padima u usluzi OneDrive

Ako OneDrive više puta pada, isprobajte ove korake za rešavanje problema:

**Uverite se da ključevi registratora nisu podešeni:**

1. Pomoću uređivača registratora pređite na HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive
2. Ako je postavka DisableFileSyncNGSC prisutna i postavljena na 1, otvorite ključ i promenite vrednost na 0.
3. Ručno pokrenite OneDrive tako što ćete otvoriti "Start" meni ![Pritisnite taster Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), otkucajte OneDrive u polju za pretragu, a zatim kliknite na OneDrive aplikaciju za računare.

**Uspostavite početne vrednosti za OneDrive:**

Napomene:

- Uspostavljanje početnih vrednosti za OneDrive prekida sve postojeće veze sinhronizacije (uključujući lični OneDrive ako je podešen).
- Nećete izgubiti datoteke ili podatke resetujući OneDrive na računaru.

**Da biste uspostavili početne vrednosti za OneDrive:**

1. Otvorite dijalog "Pokretanje" tako što biste pritisnuli Taster Windows i R.
2. Ukucaj %localappdata%\Microsoft\OneDrive\onedrive.exe /reset i kliknite na dugme U redu. Komandni prozor može se pojaviti nakratko.
3. Ručno pokrenite OneDrive tako što ćete otvoriti "Start" meni ![Pritisnite taster Windows](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC), otkucajte OneDrive u polju za pretragu, a zatim kliknite na OneDrive aplikaciju za računare.

Napomene:

- Ako ste odabrali da sinhronizujete samo neke fascikle pre reset pošte, morate to da uradite ponovo kada se sinhronizacija završi. Pročitajte [stavku Odaberite koje Fascikle za OneDrive treba sinhronizovati sa računarom](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85)   za više informacija.
- Morate ovo da dovršite za lični OneDrive i OneDrive for Business.