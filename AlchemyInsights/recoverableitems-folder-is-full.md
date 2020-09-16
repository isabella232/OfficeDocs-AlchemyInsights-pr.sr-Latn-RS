---
title: 1336 fascikla "stavke".
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
ms.openlocfilehash: 6ae608b776332402fe333315f5e4ff6072b0a651
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47741281"
---
# <a name="the-recoverable-items-folder-is-full"></a>Fascikla "stavke koja se može spasti" je popunjena

Za Exchange online Poštanske sandučiće, podrazumevano ograničenje prostora za skladištenje stavki je 30 GB. Ograničenje skladišta za fasciklu "stavke koje se mogu spasti" automatski se povećava na 100 GB ako je poštansko sanduče postavljeno na čekanje, eDiscovery ili se dodeljuje smernicama za zadržavanje.

Kada fascikla "Oporune stavke" dostigne ograničenje skladišta, funkcionalnost poštanskog sandučeta utiče na sledeće načine:

- Korisnik ne može da izbriše stavke iz poštanskog sandučeta.

- Pomoćnik kontrolisane fascikle ne može da izbriše stavke na osnovu postavki za zadržavanje ili kontrolisane fascikle.

- Za Poštanske sandučiće sa omogućenim oporavkom za oporavak stavki ili se stavljaju na čekanje, proces zaštite stranice kopiranja i pisanja ne može da održi verzije stavki koje uređuje korisnik.

- Za Poštanske sandučiće sa omogućenim evidentiranju nadzora poštanskog sandučeta, ne mogu se sačuvati datoteke evidencije nadzora u prijemnom poštanskom sandučetu u fascikli "stavke koje se mogu spasti".

Za Poštanske sandučiće koji nisu na čekanju, administratori mogu da koriste `Search-Mailbox -SearchDumpsterOnly -DeleteContent` komandu u usluzi Exchange online PowerShell za brisanje stavki u fascikli "stavke koje se mogu spasti". Više informacija potražite u sledećim temama:

- [Pretraga i brisanje poruka](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messagesadmin-help)

- [Pretraga – poštansko sanduče](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

Za Poštanske sandučiće na čekanju, administratori moraju da uklone čekanje pre nego što mogu da izbrišu stavke iz fascikle "stavke koje se mogu spasti". Više informacija potražite u članku [Brisanje stavki u fascikli "pristupačnije stavke" sa poštanskim sandučićima zasnovanim na oblaku](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).

Da bi se sprečilo da fascikla sa ispravnošću može da postane puna, administratori mogu da povećaju ograničenje skladišta stavki "Oporadne stavke" za Poštanske sandučiće na čekanju i podesite smernice za zadržavanje poštanskog sandučeta koje pomeraju stavke iz fascikle "Oporadne stavke" u skladište primaoca. Pogledajte članak povećanje kvote pristupačnih [stavki za Poštanske sandučiće na čekanju](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold).
