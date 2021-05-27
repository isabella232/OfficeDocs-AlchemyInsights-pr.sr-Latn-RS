---
title: Rešavanje problema sa rešavanjem problema čuva greške
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/20/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11274"
- "3200003"
ms.openlocfilehash: 1df2b7153cac99419adc4f72b1c3732e7c746eac
ms.sourcegitcommit: 730efbac8eec016b2b4f83f1b0e01e077f28c444
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 05/20/2021
ms.locfileid: "52676281"
---
# <a name="troubleshooting-ediscovery-holds-errors"></a>Rešavanje problema sa rešavanjem problema čuva greške

Imate problema sa zadržavanjem e-discovery? Evo nekih najboljih praksi koje treba da razmotrite:

- Proverite status distribucije zadrške.  Ako je status On **(na čekanju)** ili **Isključeno (na čekanju),** sačekajte da se distribucija zadrške dovrši.
- Objedinite e-discovery držite ispravke u jednom masovnom zahtevu umesto da više puta ažurirate smernice za svaku transakciju.
- Pokrenite Set-CaseHoldPolicy <policyname> -RetryDistribution u PowerShell centru za bezbednost i usaglašenost. Više detalja možete [da Povezivanje u Centar za & usaglašenost za PowerShell.](/powershell/exchange/connect-to-scc-powershell)

Korake za proveru ovih postavki i dodatnih najboljih praksi za ublažavanje i [](/microsoft-365/compliance/hold-distribution-errors)rešavanje problema sa čuvanjem e-discovery pogledajte u odeljku Rešavanje problema sa čuvanjem e-otklanjanja.
Informacije o rešavanju drugih uobičajenih problema sa e-disciklanjem potražite u članku Istraživanje, rešavanje uobičajenih problema [sa e-disciklanjem i rešavanje problema sa e-distribucijom.](/microsoft-365/compliance/ediscovery-troubleshooting-common-issues)
