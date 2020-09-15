---
title: Pretraga sadržaja nema rezultata
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
- "9000661"
- "2527"
ms.openlocfilehash: 1e90c403556a317ff810971ccfa4a91694fb1171
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47680661"
---
# <a name="no-results-from-content-searchexports"></a>Nema rezultata pretrage sadržaja/izvoza

Problemi sa pretraživanjem sadržaja/izvozom koji se ne vraća, mogu da budu uzrok određenog bezbednosnog proizvoda koji je podesio određeni administrator i da se ne javlja svim administratorima.

Da biste rešili ovo, pogledajte da li postoje filteri za bezbednost usaglašenosti koji možda uzrokuju sledeće:
1. Povezivanje sa PowerShell centra za bezbednost i usaglašenost
2. Uradite sledeće zapovesti:
<br>$org = "yourdomain.com"
<br>Filter za $org