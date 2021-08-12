---
title: Teams programski dodatak za Mac
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/10/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6173"
- "6166"
- "9003233"
- "9002573"
ms.openlocfilehash: c9c4eb811c93f6d11ebf606ba4bd20cddc2901d6616700ebfe6ef597dd8dc006
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "53940689"
---
# <a name="teams-add-in-for-mac"></a>Teams programski dodatak za Mac

Da biste rešili probleme sa Teams koji nedostaje za korisnike operativnog sistema Mac, pratite ove korake:

**1. korak:** Ako imate Exchange hibridnu potvrdu identiteta (2016 CU3 ili kasnije obavezno), koristite alatku Test-HMA.ps1 da biste potvrdili da je hibridna moderna potvrda identiteta ispravno konfigurisana. Više informacija potražite u članku [Provera valjanosti instalacije hibridne moderne potvrde identiteta za Outlook za iOS i Android.](https://aka.ms/TestHMAEAS)  

**Napomišite** Koristite FORMAT UPN adrese (na primer [username@contoso.com](mailto:username@contoso.com)), ne domen\korisničko ime. Ovo radite čak i za korisnike sa Exchange Online poštanskim sandučićima.

**2. korak:** Kada korisnik ode na **Alatke**  >  **Nalozi...** u Outlook za Mac, pronađite i izaberite nalog. Potvrdite da je navedeno korisničko ime u UPN formatu (na [primer, username@contoso.com](mailto:username@contoso.com)).

**3. korak:** Potvrdite da je korisnik Microsoft Teams licenciran. Korisnik mora da koristi pretplatu na Office 365 Za Mac, verziju proizvoda 16.24 ili noviju.