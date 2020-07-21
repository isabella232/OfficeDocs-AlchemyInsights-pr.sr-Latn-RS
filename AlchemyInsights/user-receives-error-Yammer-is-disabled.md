---
title: Korisnik prima grešku AADSTS7000112 Yammer je onemogućen
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6010"
- "9003111"
ms.openlocfilehash: c92b09ee9a9ca06f85906e7fce601582a7e83244
ms.sourcegitcommit: c078058ee0b77ee1f1496feb2f3a5773e3e3b30d
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 07/16/2020
ms.locfileid: "45198373"
---
# <a name="user-receives-error-aadsts7000112-yammer-is-disabled"></a>Korisnik prima grešku AADSTS7000112 Yammer je onemogućen

Ako dobijete poruku o pogrešci "AADSTS7000112: Application ' 00000005-0000-0ff1-CE00-000000000000" (Yammer) je onemogućen ", postoji problem sa direktorom usluge u okviru" Azure oglasa ". Administrator je možda onemogućio direktora usluge da bi blokirao pristup mreži Yammer.

Onemogućavanje glavnice usluge se ne preporučuje i može izazvati dodatne probleme. Više informacija o podržanom pristupu za blokiranje korisničkog pristupa Yammer potražite [u članku isključivanje pristupa na mreži za korisnike kompanije Microsoft 365](https://docs.microsoft.com/yammer/manage-yammer-users/turn-off-user-access).  

Da biste otklonili ovaj problem na Azure portalu i vratili korisnički pristup na Yammer:

1.  Otvorite stranicu "Azure Active Directory" i izaberite **poslovne aplikacije** u okviru stavke " **Upravljanje** " u levom oknu za navigaciju.
3.  U polje za pretragu otkucajte **Office 365 Yammer** , a zatim izaberite ime aplikacije da biste otvorili postavke.
4.  Izaberite **Svojstva** u okviru " **Upravljanje** " u levom oknu za navigaciju.
5.  Podesite vrednost **omogućenog za korisnike da se prijave?** na **da**, a zatim kliknite na dugme **Sačuvaj**.
6.  Ponovo se prijavite na Yammer. Možda će biti potrebno da obrišete kolačiće.

Druga mogućnost je da pokrenete komande PowerShell da biste postavili vrednost. Za više informacija, pogledajte ["Izvini, ali imamo problema sa prijavljivanjem" kada kliknete na pločicu "Yammer" u sistemu Office 365](https://docs.microsoft.com/yammer/troubleshoot-problems/error-when-click-the-yammer-tile-in-office-365). 