---
title: Lociranje izgubljenih iOS uređaja sa Intune
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
- "1283"
- "6700008"
ms.openlocfilehash: faaea65c7edc345bb676d2fb266e20f85ba2cbe5
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 07/28/2020
ms.locfileid: "45440427"
---
# <a name="locating-lost-ios-devices-with-intune"></a>Lociranje izgubljenih iOS uređaja sa Intune

Omogućavanje gubitka režima na iOS uređaju omogućava administratoru da na zaključanom ekranu prikaže poruku i broj telefona kontakta.

Kada je izgubljen režim omogućen, administrator može da koristi radnju lociranje uređaja da bi identifikovao fizičku lokaciju uređaja.

Radnja lociranja uređaja u Intune radi sa iOS uređajima da bi prikazala lokaciju određenog uređaja na mapi.

Korišćenje ove radnje zahteva da se iOS uređaj nalazi u:

- Nadgledan režim
- Izgubljeni režim

Više informacija potražite u članku [Omogućavanje izgubljenog režima na iOS/iPadOS uređajima sa Intune](https://docs.microsoft.com/intune/device-lost-mode) i [Lociranje izgubljenih ili ukradenih iOS/Ipados uređaja sa Intune](https://docs.microsoft.com/intune/device-locate).

**NAJČEŠĆA PITANJA**

Q: izdao sam udaljenu radnju da biste uklonili podatke o preduzeću sa uređaja, a sada je zaglavljeno u stanju čekanja.

A: da bi se udaljena radnja uspešno dovršila, ciljni uređaj mora biti na mreži i zdrav. U sledećim situacijama, udaljena radnja ostaje u stanju čekanja 30 dana ili dok uređaj ne bude priznao komandu:

- Kada uređaj nema vezu
- Kada uređaj izgubi status upravljanja sa Intune

Ako mislite da se uređaj više ne proverava i da neće moći da ukloni podatke o preduzeću, izaberite opciju "Izbriši". Brisanje uklanja zapis uređaja tako da se više ne pojavljuje na listi za Intune uređaja. Ako uređaj ponovo postane aktivan, korisnik će morati da je ponovo prijavi.

Q: Zašto određene udaljene radnje nisu dostupne da bi se koristila?

A: ne podržavaju sve platforme sve radnje udaljenog uređaja. Sledeće udaljene radnje su karakteristične za platformu, tako da su dostupne samo za platforme koje su obeležene.

- Zaobiđi zaključavanje aktivacije (samo iOS)
- Novi početak (samo za Windows)
- Izgubljeni režim (samo iOS)
- Lociranje uređaja (samo iOS)
- Ponovo pokreni (samo za Windows)

Više detalja o svakoj radnji potražite u članku [Dostupne radnje uređaja](https://docs.microsoft.com/intune/device-management#available-device-actions).