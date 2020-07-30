---
title: Premeštanje e-poruka u poštansko sanduče arhive
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 9af8a4d3ce72fd901ff2f3a1aae0654c7213dd7e
ms.sourcegitcommit: ffbed67c0a16ec423fa1d79b71e48ea4e2d320e1
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 07/29/2020
ms.locfileid: "46522785"
---
# <a name="move-email-to-the-archive-mailbox"></a>Premeštanje e-poruke u poštansko sanduče arhive

Ako želite da pokrećemo automatske provere za gore pomenute postavke, kliknite na dugme "nazad" <--na vrhu ove stranice, a zatim unesite e-adresu korisnika koji ima problema prilikom premeštanja e-pošte u poštansko sanduče arhive.

1. Potvrdite da je **poštansko sanduče arhive** omogućeno. Ako ne, koristite korake iz [ovog članka](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) da biste omogućili poštansko sanduče arhive.

2. Da bi se poruke automatski arhivirali u poštansko sanduče arhive, oznaka za zadržavanje sa radnjom " **Premesti u arhivu** " mora biti podešena tako da se **automatski primenjuje u celokupnu oznaku "poštansko sanduče" (podrazumevana)**. Koristite korake ovde da biste kreirali oznaku: [Arhiviraj podrazumevanu oznaku](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).

3. Zatim dodajte oznaku **arhive** u smernice za zadržavanje. U Exchange admin Center izaberite smernice za **zadržavanje** > dodajte stavku " **Premesti u** " u smernicu > " **Sačuvaj**".

4. Sada [dodelite smernice za zadržavanje](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) u poštansko sanduče određenog korisnika. Ista smernica će se primeniti i na **primarnu** i u poštansko sanduče **arhive** .

Možda će biti neophodno da naterate pomoćnika za upravljane fascikle (MFA) da pokrećete i primenite nove postavke na korisnikovo poštansko sanduče. Pokrenite sledeću komandu dok [ste povezani sa EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) da biste pokrenuli pomoćnika za kontrolisanu fasciklu za određeno poštansko sanduče:
  
Start-ManagedFolderAssistant-identitet<name of the mailbox>

Više informacija o podešavanju smernica arhive potražite [u članku Podešavanje smernica za arhiviranje i brisanje za Poštanske sandučiće](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).
  