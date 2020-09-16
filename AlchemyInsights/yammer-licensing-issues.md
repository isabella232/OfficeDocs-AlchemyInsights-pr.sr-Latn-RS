---
title: Problemi sa licenkom Yammer
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
ms.openlocfilehash: f0a7625c7b77860e5ba0e29f2df47101749aace3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47657290"
---
# <a name="yammer-licensing-issues"></a>Problemi sa licenkom Yammer

Svi korisnici moraju da imaju licencu za korišćenje usluge Yammer Enterprise, ali podrazumevano Yammer ne zahteva da korisnici imaju licencu za pristup usluzi. Kada administrator promeni postavku tako da blokira Microsoft 365 korisnike bez Yammer licenci, korisnici koji nemaju Yammer Enterprise licencu ne mogu da pristupe Yammer usluzi. Više informacija potražite u članku [Upravljanje korisničkim licencama usluge Yammer u sistemu Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365) 

Kada se licence uklone sa korisnika, pločica Yammer više se ne prikazuje, a druge usluge mogu da koriste uklanjanje licenci za skrivanje funkcija. U drugim slučajevima, funkcije se i dalje mogu pojavljivati, ali zahtevaju da se zadatak licence radi.  

**Licenca se ne ažurira za korisnika**  

Povremeno je korisniku dodeljena licenca, ali još uvek ne može da pristupi Yammeru. Kašnjenje se može pojaviti kada je u toku dodela masovne licence. Yammer korisnici se možda neće ažurirati istim redosledom kao što se licence menjaju u usluzi Azure AD zato što se sistem asinhrono pokreće. Sačekajte 24 časa pre otvaranja slučaja podrške da biste prijavili probleme sa sinhronizacijom licence.  

**Dodela masovne licence**  

Licence se mogu dodeliti administratorskom centru ili PowerShell Scripting. Više informacija potražite u članku [dodeljivanje licenci korisnicima](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) i [dodeljivanje licenci korisničkim nalozima pomoću usluge Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell). 

Microsoft podrška ne pruža pomoć za kreiranje skripti, ali je dostupna dokumentacija za Yammer zadatak licence. Više informacija potražite u članku [Upravljanje uslugom Yammer pomoću programa Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).