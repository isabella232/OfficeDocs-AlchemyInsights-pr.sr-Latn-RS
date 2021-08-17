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
ms.openlocfilehash: d4615d335b9aeef69148cd93ff9f44bec6d7d876
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/13/2021
ms.locfileid: "58314218"
---
# <a name="active-directory-not-syncing"></a>Active Directory se ne sinhronizuje

Ako dobijate greške prilikom sinhronizacije, na primer "nema nedavne sinhronizacije" ili primetite da status sinhronizacije direktorijuma na Kancelarija portalu za adminitre kaže "Poslednji put sinhronizovano pre više od 3 dana", moguće je da AADConnect ima neispravne postavke ili nedovoljne dozvole za izvršavanje sinhronizacije.  

Poništavanje usluge AADConnect pomoću ekspresnih postavki može brzo da reši problem:

1. [Preuzmite najnoviju verziju AADConnect.](https://go.microsoft.com/fwlink/?LinkId=615771)

2. [Pratite uputstva za ekspresnu instalaciju](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).

Azure AD Connect mora da se instalira na Windows serveru 2012 ili novijoj verziji. Ovaj server mora da bude pridružen domenu i može da bude kontroler domena ili server član. Kompletnu listu zahteva i preduslova za Azure AD Povezivanje, pregledajte preduslove za [Azure AD Povezivanje.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-prerequisites)

Više informacija o AADConnect nalozima usluge potražite u temi [Azure AD Povezivanje: Nalozi i dozvole.](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions)
