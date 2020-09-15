---
title: Aktivni direktorijum se ne sinhronizuje
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001688"
- "3754"
ms.openlocfilehash: 3517f424b4dcd89f915acebab747a9bff993fdbd
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47697643"
---
# <a name="active-directory-not-syncing"></a>Aktivni direktorijum se ne sinhronizuje

Ako primate greške sinhronizacije, kao što je "nije došlo do nedavne sinhronizacije" ili primetite da status sinhronizacije direktorijuma na Office administratorskim portisima piše, "poslednji put sinhronizovan pre više od 3 dana", može biti da AADConnect ima neispravne postavke ili nije imala dovoljne dozvole za sinhronizaciju.  

Ponovna instalacija AADConnect pomoću postavki Ekspresna može brzo rešiti problem:

1. [Preuzmite najnoviju verziju programa AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).

2. [Izvršite uputstva za ekspresnu instalaciju](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).

Više informacija o AADConnect nalozima usluge potražite u članku [Azure AD Connect: nalozi i dozvole](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).
