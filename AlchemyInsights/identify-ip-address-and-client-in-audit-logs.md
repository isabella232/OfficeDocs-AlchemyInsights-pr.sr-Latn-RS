---
title: Identifikovanje IP adrese i klijenta u evidenciji nadzora
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
ms.openlocfilehash: 295418f3c433df2ba1004f4bec4377c68e6bb155
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47668324"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a>Identifikovanje IP adrese i klijenta u evidenciji nadzora

IP adresa koja odgovara aktivnosti Microsoft 365 korisnika ili administratora je prikazana u evidenciji nadzora. Informacije o klijentu se takođe evidentiraju. Evo koraka za identifikovanje takvih informacija

1. Prijavite se u [Microsoft 365 Security & centar za usaglašenost](https://protection.office.com/).

2. Idite na stranicu **Search**  >  **Pretraga evidencije nadgledanja** za pretraživanje.

   Ako ste zainteresovani za određenu aktivnost, izaberite je sa liste **aktivnosti** . Ako to ne uradite, sve aktivnosti će biti vraćene za izabranog korisnika (podrazumevana postavka).

   **Napomena**: neke aktivnosti možda neće biti dostupne u meniju " **aktivnosti** "; Međutim, te stavke nadgledanja će biti vraćene ako je izabrana opcija **Prikaži rezultate za sve aktivnosti** (podrazumevana postavka).

3. Navedite korisničko ime u polju **Korisnici** , izaberite odgovarajući opseg datuma za aktivnost, a zatim kliknite na dugme **Pretraži**.

U rezultatima možete da vidite IP adresu za tu aktivnost u oknu sa rezultatima. Izaberite zapis nadzora da biste videli detaljne informacije u razgledanju **detalja** (na primer klijenta, korisnika koji je izvršio radnju itd.).

Više informacija potražite u članku [PRONALAŽENJE IP adrese računara korišćenog za pristup kompromitovanim nalozima](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account).
