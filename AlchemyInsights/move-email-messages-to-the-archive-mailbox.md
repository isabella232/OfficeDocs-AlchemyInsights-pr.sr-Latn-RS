---
title: Premeštanje e-poruka u arhivski poštansko sanduče
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
ms.openlocfilehash: 7e72766f441e210a81fcfd6c07b1801f6c0474afb02a70edf2ad8dbb571f3d2a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "53974971"
---
# <a name="move-email-to-the-archive-mailbox"></a>Premeštanje e-pošte u arhivski poštansko sanduče

Ako želite da pokrenemo automatske provere postavki koje su pomenute ispod, kliknite na dugme "nazad< – na vrhu ove stranice, a zatim unesite adresu e-pošte korisnika koji ima problema sa premeštanjem e-pošte u svoje arhivno poštansko sanduče.

1. Potvrdite da **je omogućeno Arhivno** poštansko sanduče. Ako ga ne koristite, koristite korake [u ovom članku](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) da biste omogućili arhiviranje poštanskog sandučeta.

2. Da biste automatski arhivirao poruke u arhivskom poštanskom sandučetu, oznaka zadržavanja sa radnjom Premesti u arhivu mora da se podesi da se automatski primeni na celo poštansko sanduče **(podrazumevano) oznaku**.  Koristite korake ovde da biste kreirali oznaku: [Arhiviranje podrazumevane oznake](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).

3. Zatim **dodajte oznaku** Arhiva u smernice za zadržavanje. U Exchange za zadržavanje odaberite stavku Smernice za zadržavanje **>** dodate oznaku Premesti u arhivu u smernice >  **Sačuvaj**.

4. Sada [dodelite smernice za zadržavanje](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) poštanskom sandučetu određenog korisnika. Iste smernice će se primeniti i na **primarno** i **na arhivno poštansko** sanduče.

Možda će biti neophodno da navedete kontrolisanog pomoćnika za fascikle (MFA) da se pokrene i primeni nove postavke u poštanskom sandučetu korisnika. Pokrenite sledeću komandu [dok ste povezani sa funkcijom EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) da biste pokrenuli pomoćnik za kontrolisane fascikle za određeno poštansko sanduče:
  
Start-ManagedFolderAssistant -Identity <name of the mailbox>

Dodatne informacije o podešavanju smernica za arhiviranje potražite u temi Podešavanje smernica za arhiviranje i brisanje [za poštanske sandučiće.](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users)
  