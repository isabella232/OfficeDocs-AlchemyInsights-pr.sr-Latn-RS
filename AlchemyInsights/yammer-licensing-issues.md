---
title: Problemi sa licenciranjem Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5900"
- "9003071"
ms.openlocfilehash: 6d9b2126dc1ed90968738ddb2e249dce9857f1db
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148319"
---
# <a name="yammer-licensing-issues"></a>Problemi sa licenciranjem Yammer

Svi korisnici moraju da imaju licencu za korišćenje usluge Yammer Enterprise, ali podrazumevano nije potrebno da korisnici imaju licencu za pristup usluzi. Kada administrator promeni postavku za blokiranje Microsoft 365 korisnika bez licenci za Yammer, korisnici nisu dodelili licencu za Yammer Enterprise, ne mogu da pristupe usluzi Yammer. Više informacija potražite u članku [Upravljanje korisničkim licencama za Yammer u sistemu Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365) 

Kada se licence uklone od korisnika, pločica Yammer više nije prikazana, a druge usluge mogu da koriste uklanjanje licence za skrivanje funkcija. U drugim slučajevima, funkcije se i dalje mogu pojaviti, ali zahtevaju dodelu dozvole za rad.  

**Licenca se ne ažurira za korisnika**  

Korisniku se povremeno dodeljuje licenca, ali i dalje ne može da pristupi mreži Yammer. Verovatnije je da će doći do kašnjenja kada je dodela masovne dozvole u toku. Korisnici mreže Yammer možda neće biti ažurirani u istom redosledu u kome se licence menjaju u Azure OGLASU jer se sistem asinhrono pokreće. Sačekajte do 24 sata pre nego što otvorite predmet podrške da biste prijavili probleme sa sinhronizacijom licence.  

**Dodeljivanje masovne dozvole**  

Licence se mogu dodeliti putem administratorskog centra ili skriptovanja PowerShell. Više informacija potražite u članku [dodeljivanje licenci korisnicima](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) i [dodeljivanje licenci korisničkim nalozima pomoću sistema Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell). 

Microsoft podrška ne pruža pomoć pri kreiranju skripti, ali je dostupna dokumentacija o dodeljnoj dodeli licenci za Yammer. Više informacija potražite u članku [upravljanje licencama za Yammer pomoću Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).