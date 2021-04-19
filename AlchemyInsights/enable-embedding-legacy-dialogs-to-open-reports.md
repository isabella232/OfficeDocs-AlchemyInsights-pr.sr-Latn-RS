---
title: Omogućavanje ugrađivanje zakasnelih dijaloga za otvaranje izveštaja
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002931"
- "5612"
ms.openlocfilehash: c8a5634d5d79cbd584284b675e5db4e448a0d157
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814278"
---
# <a name="enable-embedding-legacy-dialogs-to-open-reports"></a>Omogućavanje ugrađivanje zakasnelih dijaloga za otvaranje izveštaja

**Simptom**

Korisnici ne mogu da otvore izveštaje. "Nešto nije u redu. Proverite tehničke detalje za više detalja".

**Uzrok**

Izveštaji ne uspevaju da se učitaju u UCI sa greškom "Opis obrasca je bez vrednosti ili nije definisan". Izveštaji u UCI i dalje zahtevaju zakasnele dijaloge, tako da sistem klijenta mora da ima omogućeni *allowlegacydialogsembebedding.*

**Rešenje**

1. Idite na **karticu Postavke >Administracija > Postavke sistema > Opšte postavke.**

2. Postavite opciju "Omogući ugrađivanje određenih zatamnjenih dijaloga u klijentu pregledača "Ujedinjeni interfejs" na **da.**
