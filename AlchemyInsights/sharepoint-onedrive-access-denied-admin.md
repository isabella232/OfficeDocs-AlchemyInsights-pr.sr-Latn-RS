---
title: Rešavanje problema sa pristupom "zabranjen pristup"
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 3189fa61d28253569278024d4191ee63b917509f
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/10/2021
ms.locfileid: "50707968"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>Rešavanje problema sa pristupom zabranjen poruka u sistemu SharePoint/OneDrive centar administracije

Ako dobijate poruku o zabranjeni pristup prilikom pokušaja da posetite SharePoint/OneDrive centar administracije, uverite se da ste [korisniku dodelili licencu](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users). Ako korisnik ima licencu, trebalo bi da se uverite da su im [dodeljene uloge administratora](https://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) koje mogu da pristupe administratorskim centrima.

Ovaj problem takođe može da se pojavi kada se korisnik izbriše i ponovo kreira sa istim direktorom glavnog imena (UPN). Novi nalog se kreira pomoću različitog korisničkog polja (Passport unikatni ID). Kada korisnik pokuša da pristupi kolekciji lokacija ili svom OneDrive, korisnik ima neispravni PUID. Drugi scenario uključuje sinhronizaciju direktorijuma sa organizacionim jedinicama aktivnog direktorijuma (OU). Ako su se korisnici već prijavili u sistemu SharePoint, a zatim se premeštaju u drugačiji a i ponovo sinhronizuju sa sistemom SharePoint, oni mogu da doћive ovaj problem.

Da biste rešili ovaj problem, trebalo bi da vratite originalni UPN sa koracima u članku, [vratite korisnika u prethodno stanje u usluzi Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).

Napomena: ako OneDrive ili SharePoint centar administracije nisu dostupni većem broju korisnika koji su prethodno imali Access, možda postoji privremeno izdanje.  [Potvrdite izbor u polju za zdravstvenu zaštitu usluge](https://portal.office.com/adminportal/home#/servicehealth).


