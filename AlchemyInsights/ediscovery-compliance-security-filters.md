---
title: Nisu vraćeni rezultati tokom pretrage/izvoza sadržaja
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3200003"
- "7463"
ms.openlocfilehash: 5c04364f98dccbcad0f011df866f137d79c166ad3839b408d6be447d50a87ac3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "54101280"
---
# <a name="no-results-returned-during-content-searchexport"></a>Nisu vraćeni rezultati tokom pretrage/izvoza sadržaja

Ako imate problema sa sledećim scenarijima e-discovery:

- Pretraga/izvoz sadržaja ne vraća nikakve podatke ili neočekivane podatke
- Pretraga e-discovery ili izvoz nisu uspeli

To može da bude zbog određenih filtera za bezbednost usaglašenosti koje je instalirao određeni administator i koji nisu preneti svim administancima.

Da biste rešili ovo, proverite da li postoje filteri za bezbednost usaglašenosti koji možda izazivaju ove probleme:

1. Povezivanje powershell centra za bezbednost i usaglašenost
2. Pokrenite sledeće komande:

    `$org = “yourdomain.com”`

    `Get-ComplianceSecurityFilter -Organization $org`

Dodatne informacije o filterima za bezbednost usaglašenosti potražite u temi [Filtriranje dozvola za pretragu sadržaja](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)
