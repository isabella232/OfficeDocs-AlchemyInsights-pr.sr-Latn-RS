---
title: Active Directory se ne sinhronizuje
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
- "9001688"
- "1300023"
- "3754"
- "4531"
ms.openlocfilehash: 0da512379e5a2f6ccb773e18c465e545c0660560
ms.sourcegitcommit: e42bb24c9bae1d0df8c49c424d2aa5e7466703ac
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 06/14/2021
ms.locfileid: "52930989"
---
# <a name="active-directory-not-syncing"></a>Active Directory se ne sinhronizuje

Ako primate greške prilikom sinhronizacije, na primer "nema nedavne sinhronizacije" ili primetite da status sinhronizacije direktorijuma na Kancelarija portalu za adminitre kaže "Poslednji put sinhronizovano pre više od 3 dana", moguće je da AADConnect ima neispravne postavke ili nedovoljne dozvole za izvršavanje sinhronizacije.  

Poništavanje usluge AADConnect pomoću ekspresnih postavki može brzo da reši problem:

1. [Preuzmite najnoviju verziju AADConnect.](https://go.microsoft.com/fwlink/?LinkId=615771)

2. [Pratite uputstva za ekspresnu instalaciju](/azure/active-directory/hybrid/how-to-connect-install-express).

Azure AD Connect mora da se instalira na Windows serveru 2012 ili novijoj verziji. Ovaj server mora da bude pridružen domenu i može da bude kontroler domena ili server član. Kompletnu listu Azure AD Povezivanje zahteve i preduslove, pregledajte preduslove za [Azure AD Povezivanje.](/azure/active-directory/hybrid/how-to-connect-install-prerequisites)

Više informacija o AADConnect nalozima usluge potražite u temi [Azure AD Povezivanje:](/azure/active-directory/hybrid/reference-connect-accounts-permissions)Nalozi i dozvole.
