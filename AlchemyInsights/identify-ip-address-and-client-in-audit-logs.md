---
title: Identifikovanje IP adrese i klijenta u evidencijama nadzora
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1367"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: fcad71bcc5ea6036bc8fa25a9be38caabc4d0889ee01ea86e23065333d5fce0a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "54014914"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a>Identifikovanje IP adrese i klijenta u evidencijama nadzora

IP adresa koja odgovara aktivnosti koju je Microsoft 365 ili administrator prikazala u evidencijama nadzora. Informacije o klijentu su takođe evidentirane. Evo koraka za identifikovanje takvih informacija

1. Prijavite se u Microsoft 365 [za usaglašenost.](https://protection.office.com/)

2. Idite na stranicu  >  **Pretraga evidencije nadzora pretrage.**

   Ako vas zanima određena aktivnost, izaberite je **sa liste Aktivnosti.** Ako to nije moguće, vratiće se sve aktivnosti za izabranog korisnika (podrazumevana postavka).

   **Napom:** Određene aktivnosti možda neće biti dostupne u **meniju Aktivnosti;** međutim, te stavke nadzora će biti vraćene ako se **izabere stavka Prikaži rezultate** za sve aktivnosti (podrazumevana postavka).

3. Navedite korisničko ime u **polju** Korisnici, izaberite odgovarajući opseg datuma za aktivnost, a zatim kliknite na dugme **Pretraži**.

U rezultatima ćete videti IP adresu za tu aktivnost u oknu sa rezultatima. Izaberite zapis nadzora da biste  videli detaljne informacije u iskačenom delu Detalji (na primer, Klijent, Korisnik koji je izvršio radnju itd.).

Više informacija potražite u temi [Pronalaženje IP adrese računara koji se koristi za pristup ugroženim nalogima.](/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account)
