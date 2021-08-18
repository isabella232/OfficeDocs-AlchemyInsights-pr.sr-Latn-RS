---
title: Da li vam je potrebna pomoć sa ograničenjima slanja e-pošte?
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002938"
- "5630"
ms.openlocfilehash: a13eec5d0d1abccd748653e7d7d9bb999b2e3b7a
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/13/2021
ms.locfileid: "58328840"
---
# <a name="need-help-with-email-sending-limits"></a>Da li vam je potrebna pomoć sa ograničenjima slanja e-pošte?

Ispod se nalazi **ograničenja slanja po** dizajnu koja se primenjuju u usluzi. Više informacija o ovim ograničenjima dokumentovane su [ovde.](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits)

- Da bismo odrazili isporuku nezahtevanih masovnih poruka, primenjujemo ograničenja stope primalaca po korisniku na sve odlazne i **interne poruke.** U svim SKU-ovima ovo ograničenje je **10.000 primalaca dnevno.**  Klijenti koji treba da šalju legitimnu masovnu komercijalnu e-poštu (na primer, bištani klijenata) trebalo bi da koriste nezavisne dobavljače koji su specijalizovani za te usluge.
    Napomi: Kada se dostigne ograničenje broja primalaca, poruke iz poštanskog sandučeta nije moguće slati dok broj primalaca poslatih poruka u protekla 24 časa ne padne ispod ograničenja. Korisnik neće moći da šalje poruke do tog trenutka.
- Ograničenje brzine **poruke od 30 poruka u minutu** primenjuje se na sve SKU-ove. To određuje koliko poruka korisnik može da pošalje sa svog Exchange Online naloga u navedenom periodu.
- Maksimalan broj primalaca koji su dozvoljeni u poljima **Za, Cc** i Bcc za jednu e-poruku, u svim SKU-ovima, jeste **1000 primalaca.** Da biste prilagodili ovo ograničenje, [idite ovde.](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228)
