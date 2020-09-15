---
title: Rešavanje problema sa pristupom usluzi OneDrive for Business sajtovima
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 9001cf0b7d9f1f05a2ecedca2c3137dd1b8a1c38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670630"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>Rešavanje problema sa pristupom usluzi OneDrive for Business sajtovima

Ovaj problem se najčešće javlja kada je korisnik izbrisan i ponovo kreiran sa istim direktorom glavnog imena (UPN). Novi nalog se kreira pomoću različitog korisničkog polja (Passport unikatni ID). Kada korisnik pokuša da pristupi kolekciji lokacija ili svom OneDrive, korisnik ima neispravni PUID. Drugi scenario uključuje sinhronizaciju direktorijuma sa organizacionim jedinicama aktivnog direktorijuma (OU). Ako su se korisnici već prijavili u sistemu SharePoint, a zatim se premeštaju u drugačiji a i ponovo sinhronizuju sa sistemom SharePoint, oni mogu da doћive ovaj problem.

1. Da biste rešili ovaj problem, trebalo bi da vratite originalni UPN sa koracima u članku, [vratite korisnika u prethodno stanje u usluzi Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).
2. Ako ne možete da vratite originalnog korisnika, trebalo bi da uklonite starog korisnika sa OneDrive lokacije pomoću ovih koraka, [uklonite korisnika sa liste korisničkih informacija](). 
3. Kada to uradite, korisnik može da potvrdi administratorska prava na OneDrive sajtu tako što će pratiti korake za [Dodavanje administratora u OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles) .

Više informacija o nivoima dozvola potražite u članku [Razumevanje nivoa dozvola u sistemu SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).
