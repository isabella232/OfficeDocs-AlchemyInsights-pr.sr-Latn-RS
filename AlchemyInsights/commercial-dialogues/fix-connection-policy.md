---
title: Popravljanje smernica povezivanja
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
ms.openlocfilehash: d27d570a7bc0f2c1081ba7fd52264a20bf25a453
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/13/2021
ms.locfileid: "58314858"
---
# <a name="fix-connection-policy"></a>Popravljanje smernica povezivanja

E-poruka je označena kao bezbedna i isporučena u prijemno sanduče korisnika zato što je izvorna IP adresa označena kao bezbedna u podrazumevanoj smernici filtera veze. Da biste pregledali smernice, uradite sledeće:

1. Na portalu Microsoft 365 zaštitnik , idite na odeljak Smernice za <https://security.microsoft.com/> **saradnju e-&** Smernice za saradnju & Smernice za pretnju pravilima za borbu protiv pošte u odeljku \>  \>  \>  Smernice. 

   Da biste prešli direktno na **stranicu Smernice za borbu protiv spam e-pošti,** koristite <https://security.microsoft.com/antispam> .

2. Na stranici **Smernice za borbu protiv** pošte izaberite smernicu pod imenom Smernice filtera veze **(Podrazumevano)** tako što ćete kliknuti na ime smernice.

3. U iletu detalja koji se pojavi izaberite stavku **Uredi smernicu filtera** veze u **odeljku Filtriranje** veze.

4. Pregledajte stavke u odeljku Uvek dozvoli poruke sa sledećih **IP** adresa ili opsega adresa i pogledajte da li je izabrana stavka Uključi bezbednu listu. 

   **Napomi:** Microsoft se pretplati na izvore pouzdanih pošiljalaca nezavisnih dobavljača. Ako je bezbedna lista omogućena, ovi pouzdani pošiljalaci nisu greškom označeni kao slanje poruke kao slanje. Preporučujemo da izaberete ovu opciju, jer će to smanjiti broj potvrđenih potvrđenih informacija (dobra pošta koja se klasifikova kao slanje pošte) koju primate.

Dodatne informacije potražite u [temi Konfigurisanje filtriranja veze.](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-connection-filter-policy)
