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
- "3754"
ms.openlocfilehash: 274855457a143cfccd25f9a161ff894882cee9c4
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/15/2021
ms.locfileid: "51822865"
---
# <a name="active-directory-not-syncing"></a>Active Directory se ne sinhronizuje

Ako dobijate greške prilikom sinhronizacije, na primer "nema nedavne sinhronizacije" ili primetite da status sinhronizacije direktorijuma na Portalu za office adminitre kaže "Poslednji put sinhronizovano pre više od 3 dana", moguće je da AADConnect ima neispravne postavke ili nedovoljne dozvole za izvršavanje sinhronizacije.  

Poništavanje AADConnect pomoću ekspresnih postavki može brzo da reši problem:

1. [Preuzmite najnoviju verziju AADConnect.](https://go.microsoft.com/fwlink/?LinkId=615771)

2. [Pratite uputstva za ekspresnu instalaciju](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).

Više informacija o AADConnect nalozima usluge potražite u temi [Azure AD Connect: Nalozi i dozvole.](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions)
