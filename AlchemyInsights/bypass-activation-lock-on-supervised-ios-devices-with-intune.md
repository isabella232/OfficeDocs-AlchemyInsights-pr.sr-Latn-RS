---
title: Zaobilaženje zaključavanja aktivacije na nadglednim iOS uređajima sa Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1277"
- "6700008"
ms.openlocfilehash: 16be4e0cd2e47fe5d5888cbbe1380774f859e4d6
ms.sourcegitcommit: 07e56267dedfc4cec1143072c791670cbf81186b
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 07/24/2020
ms.locfileid: "45424214"
---
# <a name="bypass-activation-lock-on-supervised-ios-devices-with-intune"></a>Zaobilaženje zaključavanja aktivacije na nadglednim iOS uređajima sa Intune

Mogućnost zaobilazi zaključavanja aktivacije na iOS uređajima olakšava oporavak iz scenarija u kojem korisnik omogućava zaključavanje aktivacije na korporativnom uređaju, a zatim napušta preduzeće.

Preliminarna zahteva za zaobilaženje zaključavanja aktivacije uključuju:

- Uređaj je "nadzirao".
- Zaključavanje za aktivaciju je uspešno omogućeno uz pomoć smernica ograničenja za iOS uređaja u usluzi Intune.

Pored toga, prilikom zaobilazne zaključavanja aktivacije, trebalo bi da:

- Fizički poseduje uređaj koji je obrisan.
- Kopirajte kôd pre nego što izdate brisanje.

**Napomena:** Kôd za brisanje ne razlikuje velika i mala slova, tako da znakovi "-" nisu neophodni.

Više informacija potražite [u članku zaobilaženje zaključavanja aktivacije na nadglednim iOS uređajima sa Intune](https://docs.microsoft.com/intune/device-activation-lock-bypass).

**NAJČEŠĆA PITANJA**

Q: **izdao sam udaljenu radnju da biste uklonili podatke o preduzeću sa uređaja, a sada je zaglavljeno u stanju čekanja.**

A: da bi se udaljena radnja uspešno dovršila, ciljni uređaj mora biti na mreži i zdrav. U sledećim situacijama, udaljena radnja ostaje u stanju čekanja 30 dana, ili dok uređaj ne bude priznao komandu kada uređaj:

- Nema vezu.
- Gubi svoj status upravljanja sa Intune.

Ako mislite da se uređaj više ne proverava i da neće ukloniti podatke o preduzeću, kliknite na dugme "Izbriši". Brisanje uklanja zapis uređaja tako da se više ne pojavljuje na listi za Intune uređaja. Da bi uređaj ponovo postao aktivan, korisnik mora ponovo da upiše uređaj.

Q: **Zašto određene udaljene radnje nisu dostupne da bi se koristila?**

A: ne podržavaju sve platforme sve radnje udaljenog uređaja. Sledeće udaljene radnje su specifična za platformu.

- Zaobiđi zaključavanje aktivacije (samo iOS)
- Novi početak (samo za Windows)
- Izgubljeni režim (samo iOS)
- Lociranje uređaja (samo iOS)
- Ponovo pokreni (samo za Windows)

Više detalja o svakoj radnji potražite u članku [Dostupne radnje uređaja](https://docs.microsoft.com/intune/device-management#available-device-actions).