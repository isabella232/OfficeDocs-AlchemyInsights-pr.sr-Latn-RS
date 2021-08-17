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
ms.openlocfilehash: 9094dcdc4507f52da1dd7c95f83aa98bab1446639d2d9f52eb3a7bc849dc183c
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/11/2021
ms.locfileid: "57888420"
---
# <a name="fix-connection-policy"></a>Popravljanje smernica povezivanja

E-poruka je označena kao bezbedna i isporučena u prijemno sanduče korisnika zato što je izvorna IP adresa označena kao bezbedna u podrazumevanoj smernici filtera veze. Da biste pregledali smernice, uradite sledeće:

1. Na portalu Microsoft 365 zaštitnik , idite na odeljak Smernice za <https://security.microsoft.com/> **saradnju e-&** Smernice za saradnju & Smernice za pretnje od pravila za borbu protiv pošte u odeljku \>  \>  \>  Smernice. 

   Da biste prešli direktno na **stranicu Smernice za borbu protiv spam e-pošti,** koristite <https://security.microsoft.com/antispam> .

2. Na stranici **Smernice za borbu protiv** pošte izaberite smernicu pod imenom Smernice filtera veze **(Podrazumevano)** tako što ćete kliknuti na ime smernice.

3. U iletu detalja koji se pojavi izaberite stavku **Uredi smernicu filtera** veze u **odeljku Filtriranje** veze.

4. Pregledajte stavke u odeljku Uvek dozvoli poruke sa sledećih **IP** adresa ili opsega adresa i pogledajte da li je izabrana stavka Uključi bezbednu listu. 

   > [!NOTE]
   > Microsoft se pretplati na izvore pouzdanih pošiljalaca nezavisnih dobavljača. Ako je bezbedna lista omogućena, ovi pouzdani pošiljalaci nisu greškom označeni kao slanje poruke kao slanje. Preporučujemo da izaberete ovu opciju, jer će to smanjiti broj potvrđenih potvrđenih informacija (dobra pošta koja se klasifikova kao slanje pošte) koju primate.

Dodatne informacije potražite u [temi Konfigurisanje filtriranja veze.](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-connection-filter-policy)
