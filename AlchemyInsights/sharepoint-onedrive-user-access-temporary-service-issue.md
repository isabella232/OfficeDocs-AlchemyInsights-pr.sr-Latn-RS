---
title: Problemi sa performansama SharePoint ili OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 08bdc2527147279063e3f66a1767203e5ccdc1dd4fd8b871f2800d3f71b9a233
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "54093789"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint ili OneDrive Slow, Nedostupno ili Nedostupno za više korisnika

Ako lokacija OneDrive ili SharePoint nije dostupna većem broju korisnika koji su ranije imali pristup, možda postoji privremeni problem sa uslugom. [Proverite kontrolnu tablu za zdravstveno stanje usluge](https://portal.office.com/adminportal/home#/servicehealth).

**Dodavanje korisnika i licenca za korisnika**

Proverite da li [ste dodelili licence korisnicima u Microsoft 365 za preduzeća.](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users)


**Dodeljivanje dozvola**

Ako je korisniku dodeljena SharePoint licenca, a i dalje prima poruku o zabranjenom pristupu, uverite se da mu je dodeljen [odgovarajući nivo](https://docs.microsoft.com/sharepoint/understanding-permission-levels) dozvole.

**Razmotrite korišćenje funkcije zahteva za pristup**

Funkcija [zahteva za pristup](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) omogućava osobama da traže pristup sadržaju za koji trenutno nemaju dozvolu da ga vide.

**Dozvoljavanje prilagođene skripte može dozvati probleme sa odbijanjem pristupa**

Postoje određeni scenariji u kojima funkcija "Dozvoli *prilagođenu skriptu"* možda predstavlja pristup odbijen. Za listu funkcija na koje ovo utiče, bezbednosne mere i mogućnost onemogućavanja funkcije. Posetite [lokaciju Dozvoljavanje ili sprečavanje prilagođene skripte.](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)

