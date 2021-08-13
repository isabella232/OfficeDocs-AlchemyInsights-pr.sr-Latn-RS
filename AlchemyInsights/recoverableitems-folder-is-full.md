---
title: 1336 RecoverableItems folder is full
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
- "1336"
- "3700003"
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: 5c8d53ceabf2428f3d6d765040f1b789b6bbeda04a22dd7fde0d2d728fd17d93
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "54061770"
---
# <a name="the-recoverable-items-folder-is-full"></a>Fascikla "Stavke koje mogu da se oporave" je puna

Za Exchange Online poštanske sandučiće podrazumevano ograničenje skladišta za fasciklu "Stavke koje mogu da se oporave" je 30 GB. Ograničenje skladišta za fasciklu "Stavke koje mogu da se oporave" automatski se povećava na 100 GB ako se poštansko sanduče stavi na zadržavanje u parnicama, zadržavanje e-pošte ili se dodelite smernicama za zadržavanje.

Kada fascikla Stavke koje mogu da se oporave dostigne ograničenje skladišta, na funkcionalnost poštanskog sandučeta utiče na sledeće načine:

- Korisnik ne može da izbriše stavke iz poštanskog sandučeta.

- Pomoćnik za kontrolisane fascikle ne može da izbriše stavke na osnovu oznake za zadržavanje ili postavki kontrolisane fascikle.

- Za poštanske sandučiće koji imaju omogućen oporavak od pojedinačnih stavki ili koji se stave na čekanje, proces zaštite stranice kopiranja u pisanje ne može da održava verzije stavki koje je korisnik uredio.

- Za poštanske sandučiće koji imaju omogućeno evidentiranje nadzora poštanskog sandučeta, nijedna stavka evidencije nadzora poštanskog sandučeta ne može da se sačuva u potfascikli "Nadzori" u fascikli "Stavke koje mogu da se oporave".

Za poštanske sandučiće koji nisu na čekanju, Exchange Online programu PowerShell mogu da koriste komandu u programu PowerShell da bi izbrisali stavke iz fascikle "Stavke koje mogu da se `Search-Mailbox -SearchDumpsterOnly -DeleteContent` oporave". Dodatne informacije potražite u sledećim temama:

- [Traženje i brisanje poruka](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messagesadmin-help)

- [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

Za poštanske sandučiće koji su na čekanju, administranici moraju da uklone zadršku da bi mogli da izbrišu stavke iz fascikle "Stavke koje mogu da se oporave". Više informacija potražite u temi Brisanje stavki u fascikli "Stavke koje mogu da se oporave" u poštanskim sandučićima zasnovanim na [oblaku na čekanju.](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold)

Kako bi sprečili da fascikla "Stavke koje mogu da se oporave" postane puna, administaratori mogu da povećaju ograničenje skladišta fascikle "Stavke koje mogu da se oporave" za poštanske sandučiće na čekanju i da podese smernice za zadržavanje poštanskog sandučeta koje premeštaju stavke iz fascikle "Stavke koje mogu da se oporave" u arhivski poštansko sanduče korisnika. Pogledajte [povećavanje kvote stavki koje mogu da se oporave za poštanske sandučiće na čekanju.](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold)
