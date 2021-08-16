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
ms.openlocfilehash: e1ad34e8a5cefe168b86727ac3ca208d90f8d4478696cef58a7d0b04475fba56
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "54003403"
---
# <a name="enable-embedding-legacy-dialogs-to-open-reports"></a>Omogućavanje ugrađivanje zakasnelih dijaloga za otvaranje izveštaja

**Simptom**

Korisnici ne mogu da otvore izveštaje. "Nešto nije u redu. Proverite tehničke detalje za više detalja".

**Uzrok**

Izveštaji ne uspevaju da se učitaju u UCI sa greškom "Opis obrasca je bez vrednosti ili nije definisan". Izveštaji u UCI i dalje zahtevaju zakasnele dijaloge, tako da sistem klijenta mora da ima omogućeni *allowlegacydialogsembebedding.*

**Rešenje**

1. Idite na Postavke >**Administracija > System Postavke > General tab**.

2. Postavite opciju "Omogući ugrađivanje određenih zatamnjenih dijaloga u klijentu pregledača "Ujedinjeni interfejs" na **da.**
