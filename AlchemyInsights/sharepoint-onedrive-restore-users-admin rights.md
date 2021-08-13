---
title: Rešavanje problema sa porukama programa Access odbijen je na OneDrive for Business lokacijama
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
ms.openlocfilehash: fc4a2bd7dcc74f5f05e8b709e4bc3eac6ed445d6e2ea9ede698abbc8667723ce
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "53957807"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a>Rešavanje problema sa porukama programa Access odbijen je na OneDrive for Business lokacijama

Do ovog problema najčešće dolazi kad korisnik izbriše i ponovo ga kreira sa istim glavnim korisničkim imenom (UPN). Novi nalog se kreira pomoću druge PUID (Jedinstveni pasoš) vrednosti. Kada korisnik pokuša da pristupi kolekciji sajtova ili svojoj OneDrive, korisnik ima neispravan PUID. Drugi scenario uključuje sinhronizaciju direktorijuma sa Active Directory organizacionom jedinicom (OU). Ako su se korisnici već prijavili u uslugu SharePoint, a zatim premešteni u drugi OU i ponovo se ponovo SharePoint, može se ovaj problem rešiti.

1. Da biste rešili ovaj problem, trebalo bi da vratite originalni UPN u prethodno stanje uz korake iz ovog članka Vraćanje korisnika u prethodno [stanje Microsoft 365.](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user)
2. Ako ne možete da vratite prvobitnog korisnika u prethodno stanje, trebalo bi da uklonite starog korisnika sa OneDrive sajta pomoću ovih koraka, Uklonite korisnika sa liste [korisničkih informacija.]() 
3. Kada to završite, možete da proverite da li korisnik ima administratorska prava na sajt OneDrive tako što ćete pratiti korake za dodavanje administratora za korisničke [naloge OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles)

Više informacija o nivoima dozvola potražite u članku [Razumevanje nivoa dozvola u programu SharePoint.](https://docs.microsoft.com/sharepoint/understanding-permission-levels)
