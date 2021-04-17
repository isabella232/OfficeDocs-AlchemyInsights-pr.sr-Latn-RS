---
title: BitLocker ključevi za oporavak
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1922"
- "9000220"
ms.openlocfilehash: ec90e412302c74748e253f2e5430fa4205466f0d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820300"
---
# <a name="accessing-bitlocker-recovery-keys"></a>Pristup BitLocker ključevima za oporavak

Prilikom konfigurisanja BitLocker postavki Intune smernice za zaštitu krajnje tačke, moguće je definisati da li bitlocker informacije o oporavku treba da budu uskladištene u Azure Active Directory.

Ako je ta postavka konfigurisana, uskladišteni podaci o oporavku trebalo bi da budu vidljivi Intune adminitaru kao deo podataka zapisa o uređaju u intune uređajima na dva načina:

Uređaji - Azure AD uređaji - > "Uređaj" ILI uređaji -> Svi uređaji -> "Uređaj" -> za oporavak

Osim toga, ako postoji administrativni pristup samom uređaju, ključ za oporavak (Lozinka) može da se vidi tako što će pokrenuti sledeću komandu sa komandne linije sa punim privilegijama:

```
manage-bde -protectors c: -get
Example
Volume C: []
All Key Protectors
    TPM:
      ID: {8A5D13D6-7ED9-46C8-A74F-AC3ADF016EC8}
      PCR Validation Profile:
        0, 2, 4, 8, 9, 10, 11
    Numerical Password:
      ID: {DFA26333-XXXX-402C-YYYY-A8C40AF3ZZZZ}
      Password:
        393943-22222-281721-555554-577984-77777-194700-99999
```
Ako je uređaj šifrovan pre upisanja u Intune, ključ za oporavak je možda povezan sa "Microsoft nalogom" (MSA) koji se koristi za prijavljivanje na uređaj tokom OOBE procesa. Ako je to slučaj, pristupanje tom MSA uređaju i prijavljivanje sa njim trebalo bi da pokazuje uređaje za koje su uskladišteni  https://onedrive.live.com/recoverykey ključevi za oporavak.
 
Ako je uređaj šifrovan kao rezultat konfiguracije putem smernica grupe zasnovane na domenu, informacije o oporavku mogu da budu uskladištene u prethodnom sistemu Active Directory.

Ako ste konfigurisali smernice za zaštitu krajnje tačke tako da skladište ključ za oporavak u Azure Active Directory, ali ključ za određeni uređaj nije otpremen, možete da pokrenete otpremanje tako što ćete rotirati ključ za oporavak za taj uređaj sa MEM konzole. Za detalje pogledajte [rotiranje BitLocker ključeva za oporavak.](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#view-details-for-recovery-keys)

