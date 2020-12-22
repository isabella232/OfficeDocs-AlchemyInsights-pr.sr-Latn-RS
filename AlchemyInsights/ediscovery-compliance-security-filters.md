---
title: Nije vraćen nijedan rezultat tokom pretrage/izvoza sadržaja
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
ms.openlocfilehash: 8786f11f170edb151879235e19caa38b50f3f06e
ms.sourcegitcommit: 3d662e1a1440ba74b5347896347d03bb8c8f3af5
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 12/22/2020
ms.locfileid: "49727237"
---
# <a name="no-results-returned-during-content-searchexport"></a>Nije vraćen nijedan rezultat tokom pretrage/izvoza sadržaja

Ako imate problema sa sledećim scenarijima za eDiscovery:

- Pretraga sadržaja/izvoz ne vraća podatke ili neočekivane podatke
- Pretraga e-otkrivanja ili izvoz nije uspeo

To je možda zbog određenih bezbednosnih filtera koje je postavio određeni administrator i koji nisu komunicirali sa svim administratorima.

Da biste rešili ovaj problem, uverite se da postoje filteri za bezbednost usaglašenosti koji možda uzrokuju ove probleme:

1. Povezivanje sa PowerShell centra za bezbednost i usaglašenost
2. Uradite sledeće zapovesti:

    `$org = “yourdomain.com”`

    `Get-ComplianceSecurityFilter -Organization $org`

Dodatne informacije o bezbednosnim filterima usaglašenosti potražite [u članku filtriranje dozvola za pretraživanje sadržaja](https://docs.microsoft.com/microsoft-365/compliance/permissions-filtering-for-content-search)
