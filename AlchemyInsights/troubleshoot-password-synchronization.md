---
title: Rešavanje problema sa sinhronizacijom lozinke
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: 54b5a033b7cbb99520425b31800364ed4a99a4e6
ms.sourcegitcommit: 1d01b8b48eef2d5d10c375dcf802cd36e9d6bf61
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 07/23/2020
ms.locfileid: "45387891"
---
# <a name="troubleshoot-password-synchronization"></a>Rešavanje problema sa sinhronizacijom lozinke

Da biste rešili probleme sa sinhronizacijom lozinke, počnite tako što ćete koristiti ovaj zadatak rešavanja problema u vezi sa povezivanjem da biste utvrdili zašto se lozinke ne sinhronizuju. Da biste počeli, idite na [Upravljanje direktnom sinhronizacijom](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).  

1. Otvorite novu sesiju Windows PowerShell na serveru za povezivanje sa Azure serverom, a zatim izaberite opciju " **Pokreni kao administrator** ".

2. Pokretanje set-izvršne smernice RemoteSigned ili set-izvršne smernice neograničeno.

3. Pokrenite čarobnjak za povezivanje "Azure AD".

4. Idite na stranicu "dodatni zadaci" > **rešiti problem**  >  **dalje**.

5. Izaberite " **Pokreni** " da biste otvorili meni "Rešavanje problema sa PowerShell".

6. Izaberite **Rešavanje problema sa sinhronizacijom lozinke**.

    Ovo pitanje obično znači da lozinka nije sinhronizovana za određeni korisnički nalog.

    **Notes** Sinhronizacija lozinke nije uspela ako je poslednja uspešna sinhronizacija lozinke bila pre izvesnog vremena.

Da biste dobili dodatnu pomoć za rešavanje problema sa lozinkom sinhronizacija, pogledajte odeljak [Rešavanje problema sa lozinkom lozinka za sinhronizaciju pomoću programa Azure sinhr](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).