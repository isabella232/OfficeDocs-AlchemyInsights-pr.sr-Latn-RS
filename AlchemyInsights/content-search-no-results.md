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
ms.openlocfilehash: b53534dd0666fa64e692910aa6800abab30169a97fbe567c815ce6b948381a63
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "54058016"
---
# <a name="no-results-from-content-searchexports"></a>Nema rezultata pretrage/izvoza sadržaja

Problemi sa pretragom sadržaja/izvozima koji ne vraćaju podatke mogu da budu zbog određenog filtera za bezbednost usaglašenosti koji je podstagao određeni administator i što ga nije preneo svim dobavljačima.

Da biste rešili ovo, proverite da li postoje filteri za bezbednost usaglašenosti koji možda uzrokuju ovo:
1. Povezivanje powershell centra za bezbednost i usaglašenost
2. Pokrenite sledeće komande:
<br>$org = "yourdomain.com"
<br>Get-ComplianceSecurityFilter -Organization $org