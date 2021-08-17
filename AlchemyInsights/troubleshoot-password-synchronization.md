---
title: Rešavanje problema sa sinhronizacijom lozinke
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: cb782c0d1dc396ee7a9f016afb9629a2cdee93d52f5408b7a73e576e783ebc0a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "54105772"
---
# <a name="troubleshoot-password-synchronization"></a>Rešavanje problema sa sinhronizacijom lozinke

Da biste rešili probleme sa sinhronizacijom lozinki, počnite da koristite ovaj AAD Povezivanje za rešavanje problema da biste odredili zašto se lozinke ne sinhronizuju. Da biste započeli, idite na Upravljanje [direktnom sinhronizacijom](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).  

1. Otvorite novu sesiju Windows PowerShell na Azure AD Povezivanje serveru i izaberite opciju **Pokreni kao administrator.**

2. Pokrenite Set-ExecutionPolicy Isključeno ili Set-ExecutionPolicy neograničeno.

3. Pokrenite čarobnjak za Azure AD Povezivanje AD.

4. Idite na stranicu Dodatni zadaci na > **Rešavanje**  >  **problema dalje.**

5. Izaberite **stavku Pokreni** da biste otvorili meni za rešavanje problema sa programom PowerShell.

6. Izaberite **stavku Rešavanje problema sa sinhronizacijom lozinke**.

    Problem je obično u tome što se lozinka ne sinhronizuje za određeni korisnički nalog.

    **Napomene** Sinhronizacija lozinki ne uspeva ako je poslednje uspešno sinhronizovanje lozinke bilo pre nekog vremena.

Dodatnu pomoć za rešavanje problema sa sinhronizacijom lozinki možete da vidite u odeljku Rešavanje problema sa sinhronizacijom hasha lozinki uz [Azure AD Povezivanje sinhronizaciju.](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)