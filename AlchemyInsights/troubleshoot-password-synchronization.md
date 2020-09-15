---
title: Rešavanje problema sa sinhronizacijom lozinki
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
ms.openlocfilehash: 96f63f2ae8e5de246bce7fc15a9b2c3d604f2eb8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664940"
---
# <a name="troubleshoot-password-synchronization"></a>Rešavanje problema sa sinhronizacijom lozinki

Da biste rešili probleme sa sinhronizacijom lozinki, počnite pomoću ovog zadatka za rešavanje problema sa AAD povezivanjem da biste utvrdili zašto se lozinke ne sinhronizuju. Da biste počeli, idite na [Upravljanje direktnom sinhronizacijom](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).  

1. Otvorite novu sesiju Windows PowerShell na Azure AD Connect serveru i izaberite opciju " **pokrene kao administrator** ".

2. Neograničeno je potpisano ili izvršeno izvršeno smernice za stavku radi izvršenih smernica.

3. Pokrenite čarobnjak za Azure AD Connect.

4. Idite na stranicu dodatne zadatke > **rešite problem**  >  **dalje**.

5. Izaberite stavku **pokretanje** da biste otvorili meni za rešavanje problema sa PowerShell.

6. Izaberite stavku **Rešavanje problema sa sinhronizacijom lozinki**.

    Problem je obično da se lozinka ne sinhronizuje za određeni korisnički nalog.

    **Beleške** Sinhronizacija lozinki ne uspeva ako je prethodna sinhronizacija lozinki nedavno proљla.

Dodatne pomoći za rešavanje problema sa sinhronizacijom lozinki potražite [u članku rešavanje problema sa hash sinhronizacijom lozinki pomoću usluge Azure AD Connect Sync](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).