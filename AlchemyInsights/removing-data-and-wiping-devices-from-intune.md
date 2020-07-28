---
title: Uklanjanje podataka i brisanje uređaja iz Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1279"
- "6700008"
ms.openlocfilehash: efaf111f694ab57d0435b141a6d4baad58658ed2
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 07/28/2020
ms.locfileid: "45440468"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a>Uklanjanje podataka i brisanje uređaja iz Intune

Uređaj se povlače i udaljene radnje za brisanje uređaja mogu da se koriste za uklanjanje podataka o preduzeću koje upravlja Intune ili za izvođenje fabričke početne vrednosti i vraćanje uređaja na podrazumevane postavke.

1. Prijavite se na Microsoft 365 uređaj za upravljanje uređajem i idite na **uređaje "Uređaji**  >  **All Devices**".
2. Izaberite uređaj koji želite da obrišeš.
3. Izaberite tip udaljene obrisa koji želite da uradite. Penzionisati se brišu samo organizacione informacije, dok se pune maramice vraćaju uređaj na fabričke postavke.
4. Izaberite **da** da biste potvrdili izbor. Dok se brisanje ne završi, status radnje uređaja pokazuje kao da je u stanju da se povuče.</br>
    Nakon dovršenja radnje, mobilni uređaj više nećete videti na listi upravljanog uređaja.

**Belešku** Podaci o preduzeću se ne mogu ukloniti sa uređaja koji su PRIDRUŽENI Azure OGLASU.

Za sve detalje o uticaju akcija u penziju i brisanju, uključujući ono što se zadržava i šta je izbrisano, pogledajte odeljak [Uklanjanje uređaja pomoću opcije Obriši, penzionisati ili ručno uklanjanje uređaja](https://docs.microsoft.com/intune/devices-wipe).

Da biste izbrisali sve podatke sa macOS uređaja, pogledajte odeljak [Brisanje svih podataka sa Makos uređaja](https://docs.microsoft.com/intune/device-erase).