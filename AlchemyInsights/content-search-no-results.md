---
title: Nema rezultata pretrage sadržaja
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
- "9000661"
- "2527"
ms.openlocfilehash: 0267286ca5967ee891e65343d49adf776f0322a6
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816862"
---
# <a name="no-results-from-content-searchexports"></a>Nema rezultata pretrage/izvoza sadržaja

Problemi sa pretragom sadržaja/izvozima koji ne vraćaju podatke mogu da budu zbog određenog filtera za bezbednost usaglašenosti koji je podstagao određeni administator i što ga nije preneo svim dobavljačima.

Da biste rešili ovo, proverite da li postoje filteri za bezbednost usaglašenosti koji možda uzrokuju ovo:
1. Povezivanje sa powershell centrom za bezbednost i usaglašenost
2. Pokrenite sledeće komande:
<br>$org = "yourdomain.com"
<br>Get-ComplianceSecurityFilter -Organization $org