---
title: Primer Microsoft Defender za Office 365 anti-phishing smernice
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: eabff70c22b641627d3ab6c0b2f8846a0be2f49e
ms.sourcegitcommit: 60c504f3ac187eaf1141b3ba701d9e0633bdd968
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/08/2021
ms.locfileid: "50695643"
---
# <a name="example-microsoft-defender-for-office-365-anti-phishing-policy"></a>Primer Microsoft Defender za Office 365 anti-phishing smernice

Ove postavke omogućavaju smernice zvano *domen i izvršni direktor*. Ova smernica omogućava i zaštitu korisnika i domena od imitacije, a zatim primenjuju smernice na sve e-poruke koje primaju korisnici unutar domena. Prvo dodajte sledeće informacije da biste kreirali smernice:

- **Ime**: **Opis** domena i generalnog direktora: obezbeđuje da se izvršni direktor i vaš domen ne imitiraju.
  **Primeni na**: izaberite **domen primaoca**. U okviru **bilo koje od ovih** **stavki izaberite stavku Izaberi**, a zatim izaberite domen. Izaberite stavku **+ Dodaj**. Potvrdite izbor u polju za potvrdu pored imena domena na listi (na primer, *contoso.com*), a zatim izaberite stavku **Dodaj**. Izaberite stavku **gotovo**.
- Kada se smernice kreiraju, možete precizno da kreirate smernice pomoću sledećih opcija:
  - **Dodavanje korisnika u zaštitu:** U ovom primeru, dodajte adresu e-pošte izvršnog direktora.
  - **Dodajte domeni da biste zaštitili**: dodajte organizacioni domen koji uključuje Office generalnog direktora.
  - **Odaberite stavke Radnje**: **Ako je imitator poslao e-poštu**, izaberite **poruku preusmeravanja na drugu e-adresu**, a zatim unesite e-adresu administratora bezbednosti (na primer, *securityadmin@contoso.com*). **Ako će e-pošta biti poslata pomoću imitiranog domena**, izaberite stavku **karantin**.
  - **Obaveštajna služba za poštansko sanduče**: Ova opcija je podrazumevano izabrana kada kreirate novu anti-phishing smernice. Ostavite **ovo podešavanje za** najbolje rezultate.
  - **Dodajte Pouzdane pošiljaoce i** domeni: Za ovaj primer, nemojte definisati zamene.
- Kada pregledate postavke, izaberite stavku **Kreiraj ove smernice** ili **Sačuvaj** na odgovarajući način.

Da biste saznali više, pogledajte članak [anti-phishing smernice u programu Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2092235).
