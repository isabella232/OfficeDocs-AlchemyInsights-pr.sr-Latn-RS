---
title: Yammer sa licenciranjem
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5900"
- "9003071"
ms.openlocfilehash: 3ec764ece9cb7be933e9e2cd002379898522790528b0fa586ab501424b00cd7b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "53989749"
---
# <a name="yammer-licensing-issues"></a>Yammer sa licenciranjem

Svi korisnici moraju da imaju licencu da bi koristili uslugu Yammer Enterprise, ali Yammer podrazumevano ne zahteva da korisnici imaju licencu za pristup usluzi. Kada administrator promeni postavku tako da blokira Microsoft 365 korisnike koji Yammer licence, korisnici kojima nije dodeljena licenca za Yammer Enterprise ne mogu da pristupe Yammer usluzi. Više informacija potražite u članku [Upravljanje Yammer korisničkim licencama u Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365) 

Kada se licence uklone za korisnike, pločica Yammer više se ne prikazuje, a druge usluge mogu da koriste uklanjanje licence da bi sakrile funkcije. U drugim slučajevima, funkcije se i dalje mogu pojaviti, ali zahtevaju licencu za rad.  

**Licenca se ne ažurira za korisnika**  

Korisniku se povremeno dodeljuje licenca, ali i dalje ne može da pristupi Yammer. Odlaganja se verovatno dešavaju kada je u toku masovno dodeljivanje licenci. Yammer korisnici možda neće biti ažurirani istim redosledom kao licence u Azure AD jer se sistem pokreće asimetrirani. Sačekajte do 24 časa pre nego što otvorite predmet podrške kako biste prijavili probleme sa sinhronizacijom licence.  

**Masovno dodeljivanje licence**  

Licence možete da dodelite putem centra za administracije ili PowerShell skripti. Dodatne informacije potražite u [članku Dodela licenci](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) korisnicima i Dodela licenci korisničkim nalozima Office 365 [PowerShell.](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell) 

Microsoft podrška ne pruža pomoć oko kreiranja skripti, ali je dostupna dokumentacija Yammer dodeljivanje licenci. Više informacija potražite u [članku Upravljanje Yammer licencama pomoću Windows PowerShell.](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell)