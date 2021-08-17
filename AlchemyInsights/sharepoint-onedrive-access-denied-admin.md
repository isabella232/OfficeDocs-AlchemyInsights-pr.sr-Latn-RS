---
title: Rešavanje problema sa porukama koje su odbijene za pristup
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 9acde72f82a27c9f2faa2cf4d0417374aa5a294234da96080dc0498d07639248
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "54085242"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Rešavanje problema sa pristupom odbijenim porukama u sharepoint/OneDrive centru za administaciju

Ako dobijate poruku o zabranjenom pristupu prilikom pokušaja pretraživanja Sharepoint/OneDrive centra za OneDrive, proverite da li ste dodelili licencu [korisniku.](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users) Ako korisnik ima licencu, trebalo bi da se uverite i da mu je dodeljena [uloga administratora](https://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) koja može da pristupi centrima administracije.

Do ovog problema takođe može doći kada korisnik izbriše i ponovo kreira sa istim glavnim korisničkim imenom (UPN). Novi nalog se kreira pomoću druge PUID (Jedinstveni pasoš) vrednosti. Kada korisnik pokuša da pristupi kolekciji sajtova ili svojoj OneDrive, korisnik ima neispravan PUID. Drugi scenario uključuje sinhronizaciju direktorijuma sa Active Directory organizacionom jedinicom (OU). Ako su se korisnici već prijavili u uslugu SharePoint, a zatim premešteni u drugi OU i ponovo se ponovo SharePoint, može se ovaj problem rešiti.

Da biste rešili ovaj problem, trebalo bi da vratite originalni UPN u prethodno stanje uz korake navedene u članku Vraćanje korisnika u [prethodno stanje Microsoft 365.](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user)

Najava: Ako OneDrive ili SharePoint centru za administaciju nije dostupan većem broju korisnika koji su ranije imali pristup, možda postoji privremeni problem sa uslugom.  [Proverite kontrolnu tablu za zdravstveno stanje usluge](https://portal.office.com/adminportal/home#/servicehealth).


