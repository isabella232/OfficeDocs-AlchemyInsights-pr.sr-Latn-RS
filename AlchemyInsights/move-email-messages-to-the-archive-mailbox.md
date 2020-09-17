---
title: Premeštanje e-poruka u poštansko sanduče arhive
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
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 61d0b1a58fff6655b745bb9d39e8384f0a543336
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/15/2020
ms.locfileid: "47799794"
---
# <a name="move-email-to-the-archive-mailbox"></a>Premeštanje e-pošte u poštansko sanduče arhive

Ako želite da uradite automatizovane provere za postavke navedene ispod, kliknite na dugme nazad <, na vrhu ove stranice, a zatim unesite e-adresu korisnika koji ima problema sa premeštanjem e-pošte u poštansko sanduče.

1. Potvrdite da je **arhivirane poštansko sanduče** omogućeno. Ako nije, koristite korake u [ovom članku](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) da biste omogućili Arhiviraj poštansko sanduče.

2. Da biste automatski arhivirati poruke u poštansko sanduče arhive, oznaka za zadržavanje sa akcijom " **Premesti u arhivu** " mora biti postavljena tako da se **automatski primeni na celu nalepnicu sa poštanskim sandučetom (podrazumevana vrednost)**. Koristite ove korake da biste kreirali oznaku: [Podrazumevana oznaka arhivira](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).

3. Zatim dodajte oznaku **arhive** u smernice za zadržavanje. U Exchange centru administracije odaberite smernice za **zadržavanje** > dodajte **Premeštanje u oznaku arhiviranja** na smernice > **Sačuvaj**.

4. Sada [dodelite smernice za zadržavanje](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) za poštansko sanduče određenog korisnika. Iste smernice će se primeniti i na **primarno** i u poštansko sanduče **arhive** .

Možda će biti neophodno da se korisnik kontrolisane fascikle (MFA) pokreće i primenjuje nove postavke na poštansko sanduče korisnika. Pokrenite sledeću komandu dok ste [povezani sa EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) da biste pokrenuli pomoćnika kontrolisane fascikle za određeno poštansko sanduče:
  
Start-Managedderderik-identitet <name of the mailbox>

Više informacija o podešavanju smernica za arhiviranje potražite u članku [Podešavanje smernica za arhiviranje i brisanje za Poštanske sandučiće](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).
  