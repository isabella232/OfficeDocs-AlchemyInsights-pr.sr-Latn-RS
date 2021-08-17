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
ms.openlocfilehash: d0ef27e7c03eb8bcd9de74c58a5e0398d8892a6eb0ab50944b3c2201247fa0b8
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/11/2021
ms.locfileid: "57889232"
---
# <a name="active-directory-not-syncing"></a>Active Directory se ne sinhronizuje

Ako dobijate greške prilikom sinhronizacije, kao što je "nema nedavne sinhronizacije" ili primetite status sinhronizacije direktorijuma na Kancelarija portalu za adminitre, "Poslednji put sinhronizovano pre više od 3 dana", moguće je da AADConnect ima neispravne postavke ili nedovoljne dozvole za izvršavanje sinhronizacije.  

Poništavanje usluge AADConnect pomoću ekspresnih postavki može brzo da reši problem:

1. [Preuzmite najnoviju verziju AADConnect.](https://go.microsoft.com/fwlink/?LinkId=615771)

2. [Pratite uputstva za ekspresnu instalaciju](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).

Azure AD Connect mora da se instalira na Windows serveru 2012 ili novijoj verziji. Ovaj server mora da bude pridružen domenu i može da bude kontroler domena ili server član. Kompletnu listu zahteva i preduslova za Azure AD Povezivanje, pregledajte preduslove za [Azure AD Povezivanje.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-prerequisites)

Više informacija o AADConnect nalozima usluge potražite u temi [Azure AD Povezivanje:](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions)Nalozi i dozvole.
