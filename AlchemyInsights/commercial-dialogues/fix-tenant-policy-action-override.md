---
title: Popravka smernica zakupca (zamena radnje)
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
ms.openlocfilehash: ee45e86a143719914f7a7917730d7e840e90625f
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/13/2021
ms.locfileid: "58326811"
---
# <a name="fix-tenant-policy-action-override"></a>Popravka smernica zakupca (zamena radnje)

Jedna od smernica za borbu protiv spam-pošte uticala je na ovu poruku. Da biste pregledali smernice, uradite sledeće:

1. Na portalu Microsoft 365 zaštitnik , idite na odeljak Smernice za <https://security.microsoft.com/> **saradnju e-&** Smernice za saradnju & Smernice za pretnju pravilima za borbu protiv \>  \>  \> **spama**  u odeljku Smernice.

   Da biste prešli direktno na **stranicu Smernice za borbu protiv spam e-pošti,** koristite <https://security.microsoft.com/antispam> .

2. Na stranici **Smernice** za borbu protiv bezedne e-pošti izaberite smernicu tako  što ćete kliknuti na ime smernice **(Tip** je Prilagođena smernica za borbu protiv bezalalne **e-pošti** ili "Ime" je smernica za dolaznu vezu bez-e-pošti **(Podrazumevano)**).
3. U iletu detalja koji se pojavljuje izaberite stavku **Uredi radnje** u **odeljku Radnje.**
4. U  odeljku Radnje poruke pregledajte verifikacije za bezžeznu e-pošte, Bez-pošte velike pouzdanosti **,** Phishing i **Phishing** velike pouzdanosti da biste videli da li je izabrana neka od sledećih vrednosti: 
   - **Dodavanje X-zaglavlja**
   - **Otvaranje reda za temu unapred sa tekstom**
   - **Preusmeravaj poruku na e-adresu**
   - **Brisanje poruke**
   - **Nijedna radnja**

   Moguće je da su standardne postavke **primenjene** na sve Exchange Online Protection su uticale na poruku.

Dodatne informacije potražite u [temi Konfigurisanje smernica za borbu protiv spam eOP-a u programu EOP.](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-your-spam-filter-policies)
