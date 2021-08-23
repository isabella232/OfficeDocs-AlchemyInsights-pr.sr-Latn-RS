---
title: Želite li da korporaciji Microsoft prijavite da je netačna lažna e-pošta?
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "975"
- "666"
- "3100019"
ms.openlocfilehash: d3897f24ce9a967b08a3fd15a2fdedbb3fe2a22d
ms.sourcegitcommit: f05d4caa0e657ee74d6b6e9abc88488f17d740fe
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/19/2021
ms.locfileid: "58396629"
---
# <a name="do-you-have-legitimate-messages-being-marked-as-spam"></a>Da li imate legitimne poruke koje su označene kao bezvredna pošta?

Frustrirajuće je kada legitimna e-poruka završi u fascikli "Neželjena e-pošta" ili u karantinu. Razmotrite ove uobičajene razloge za pozitivne na pogrešno:

**Zamene zakupca (najčešće)** To je u potpunosti unutar vaše kontrole da ga remediate.

Prosledite poruku na Microsoft 365 zaštitnik za analizu smernica i pravila na koje ovo utiče; Detalji o poništi dostupni su za nekoliko minuta.
Pregledajte ili izmenite smernice ili pravila kako je primenljivo. 

**Zamene krajnjih korisnika (uobičajeno)** To je u potpunosti unutar vaše kontrole da ga remediate. 

Prosledite poruku na Microsoft 365 zaštitnik za analizu smernica i pravila na koje ovo utiče; Detalji o poništi dostupni su za nekoliko minuta. 

Ako je poruka blokirana zato što je poslata sa adrese na korisnikovoj listi blokiranih pošiljalaca, zaglavlja obuhvataju verdict "SFV:BLK".

**Potvrda identiteta e-pošte pošiljalaca** To je delimično u okviru vaše kontrole da biste je remećeli.

Prosledite poruku da biste analizirali greške u potvrdi identiteta e-pošte pošiljaoca u trenutku isporuke; rezultati su dostupni u roku od jednog dana. 

Ako posedujete infrastrukturu slanja, pregledajte kako da je poravnate sa uslugama SPF, DKIM i DMARC da biste se uverili da odredišni sistemi e-pošte veruju porukama poslatim sa vašeg domena. Druga mogućnost je da se obratite pošiljaocima da bi rešili svoje DNS konfiguracije.

**Microsoft verifikacije za filtriranje** To je delimično u okviru vaše kontrole da biste je remećeli.

Prosledite poruku i prijavite je kao bezbednu; rescan rezultati su dostupni u toku jednog dana. Koristite listu dozvoljenih/blokiranih zaku e-poruka kada se ne slažete sa diktantima filtriranja u određenim situacijama. Međutim, ne bi trebalo da zaobižete Microsoft verifikacije filtriranja trajno. 

Za više informacija pogledajte:

- Omogućite krajnjim korisnicima da prosleđuju poruke korporaciji Microsoft. Microsoft koristi ove prosleđivanje kako bi poboljšao efikasnost tehnologija zaštite e-pošte i one se pojavljuju u izveštajima za prosleđivanje koje možete da koristite kao pokazatelj za ažuriranje smernica. 

- Da biste pogledali kratak video o prosleđivanje poruka na analizu, pogledajte [prosleđivanje poruka na analizu.](https://go.microsoft.com/fwlink/?linkid=2166435)

- [Koristite prosleđivanje za prosleđivanje podataka za koje se sumnja da su bezb, phish, ULlovi i datoteke korporaciji Microsoft](https://docs.microsoft.com/microsoft-365/security/office-365-security/admin-submission)

- [Upravljanje listom dozvoljenih/blokiranih zakuca](https://docs.microsoft.com/microsoft-365/security/office-365-security/tenant-allow-block-list)

- [Zaglavlja poruka za borbu protiv prijema pošte u Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/anti-spam-message-headers)

- [Zaštita od odlazne bezedne e-poruke u EOP-u](https://docs.microsoft.com/microsoft-365/security/office-365-security/outbound-spam-controls)