---
title: Primer Microsoft zaštitnik za Office 365 smernica za borbu protiv phishinga
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
ms.openlocfilehash: b59abdeea6ac9be7e498e2b1ba531e7bf611c92097fbc12237e78364dae84f35
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "54035020"
---
# <a name="example-microsoft-defender-for-office-365-anti-phishing-policy"></a>Primer Microsoft zaštitnik za Office 365 smernica za borbu protiv phishinga

Ove postavke omogućavaju smernice pod imenom *Domen i CEO*. Ove smernice pružaju zaštitu od imitiranja i domena, a zatim primenjuju smernice na svu e-poštu koju su korisnici primili u okviru domena. Prvo dodajte sledeće informacije da biste kreirali smernice:

- **Ime:** Domen i ceo **opis:** Obezbeđuje da se direktor i vaš domen ne imitiraju.
  **Primenjeno na:** **Izaberite domen primaoca je**. U **okviru Bilo koji od ovih** stavki **izaberite stavku** Odaberi , a zatim izaberite domen. Izaberite **+ Dodaj**. Potvrdite izbor u polju za potvrdu pored imena domena na listi (na primer, *contoso.com*), a zatim izaberite **stavku Dodaj**. Izaberite **Gotovo**.
- Kada se smernice kreiraju, smernicu možete fino da podesite koristeći sledeće opcije:
  - **Dodajte korisnike da biste zaštitili:** U ovom primeru dodajte barem adresu e-pošte direktora.
  - **Dodajte domene da biste** zaštitili: Dodajte domen organizacije koji uključuje kancelariju direktora.
  - Odaberite **radnje:** Za ako je e-poruku poslao imitirani **korisnik,** izaberite stavku Preusmeri poruku na drugu e-adresu **,** a zatim unesite e-adresu administratora bezbednosti *(na primer, securityadmin@contoso.com*). Ako **je e-poruku poslao imitirani domen,** izaberite **stavku Karantin poruka**.
  - **Informacije o poštanskom** sandučetu: Ova opcija se podrazumevano bira kada kreirate nove smernice za borbu protiv phishinga. Ostavite ovu postavku **na postavki "Dalje"** da biste ostvarili najbolje rezultate.
  - **Dodajte pouzdane pošiljalace i domene:** U ovom primeru ne definišite zamene.
- Kada pregledate postavke, izaberite opciju Kreiraj **ove** smernice ili **Sačuvaj, po** poklanjajuću postavku.

Da biste saznali više, pogledajte [Polise za borbu protiv phishinga u Microsoft 365.](https://go.microsoft.com/fwlink/?linkid=2092235)
