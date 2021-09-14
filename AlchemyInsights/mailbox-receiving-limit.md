---
title: Sprovođenje ograničenja za prijem poštanskog sandučeta
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/31/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13711"
- "9008580"
ms.openlocfilehash: c1ba5ab10b102680cec52f4e0740c3dd2ceaccbd
ms.sourcegitcommit: a36ec7eda49536933dc8c6f9319cf7320e8aa04d
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/31/2021
ms.locfileid: "59316036"
---
# <a name="mailbox-receiving-limit-enforcement"></a>Sprovođenje ograničenja za prijem poštanskog sandučeta

Microsoft je nedavno počeo da sprovava prag poštanskog sandučeta od 3600 poruka na čas. Dodatne informacije potražite u [Exchange Online ograničenja.](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-limits) Microsoft 365 poštanskim sandučićima koji dobijaju preko 3600 poruka u roku od jednog sata reaguju u narednih 60 minuta. 

Pored toga, primenjuje se ograničenje za parove primalaca pošiljaoca (SRP) koje blokira poruke koje primi Microsoft 365 poštansko sanduče određenog pošiljaoca. Ako jedan pošiljalac određenom primaocu pošalje preko 33% od ukupne vrednosti ili 1200 poruka po času prenošenja, počinje ograničenje za SRP i poštansko sanduče više neće prihvatati poruke od tog pošiljaoca. E-pojašnjeno:

- Ovo ograničenje je aplikacija za e-poruke primljene od drugih zakuca, iz drugih zakupu ili pošiljalaca interneta.
- Isporuka e-pošte u poštansko sanduče se blokira u narednih 60 minuta. 
- Pošiljke u ovim poštanskim sandučićima primaju izveštaj o neisporučivanja (5.2.121 ili 5.2.122) sa obaveštenjem da je poštansko sanduče premašio maksimalnu dozvoljenu vrednost isporuke. Intra-zakuca (pošta u okviru istog zakuca) nastavlja da se isporučuje.
- Kada se primeni ograničenje za SRP, poštansko sanduče primaoca nastavlja da prihvata poruke od drugih pošiljalaca.

Administratori mogu da nadgledaju trenutnu aktivnost poštanskog sandučeta tako što će pristupiti novom izveštaju i uvidu u Exchange centru administracije koji se zove "Poštanski sandučići prekoračuju ograničenja prijema". Uvid se pojavljuje samo ako zakuca ima uvredne poštanske sandučiće, dok se izveštaj uvek pojavljuje na dasci, ali je prazan, osim ako zakuca nema problem sa poštanskim sandučićima.

Dodatne informacije o ograničenjima za uvid o prijemu potražite u temi Poštanski sandučići koji premašuju ograničenja za dobijanje uvida u novi [EAC.](https://docs.microsoft.com/exchange/monitoring/mail-flow-insights/mailboxes-exceeding-receiving-limits-insights)

Više informacija o izveštaju o ograničenjima prijema koji premašuje prijem potražite u izveštaju o poštanskim sandučićima koji premašuju ograničenja prijema u novom [EAC-u.](https://docs.microsoft.com/exchange/monitoring/mail-flow-reports/mailboxes-exceeding-receiving-limits-report)