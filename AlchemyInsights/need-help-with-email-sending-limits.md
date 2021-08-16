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
ms.openlocfilehash: b55654f56ab405c93934fd1a0917f50c053b09466e877e1255adbd28db83d93f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "54097510"
---
# <a name="need-help-with-email-sending-limits"></a>Da li vam je potrebna pomoć sa ograničenjima slanja e-pošte?

Ispod se nalazi **ograničenja slanja po** dizajnu koja se primenjuju u usluzi. Više informacija o ovim ograničenjima dokumentovane su [ovde.](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits)

- Da bismo odrazili isporuku nezahtevanih masovnih poruka, primenjujemo ograničenja stope primalaca po korisniku na sve odlazne i **interne poruke.** U svim SKU-ovima ovo ograničenje je **10.000 primalaca dnevno.**  Klijenti koji treba da šalju legitimnu masovnu komercijalnu e-poštu (na primer, bištani klijenata) trebalo bi da koriste nezavisne dobavljače koji su specijalizovani za te usluge.
    - Napomi: Kada se dostigne ograničenje za stopu primaoca, poruke iz poštanskog sandučeta nije moguće slati dok broj primalaca poslatih poruka u protekla 24 časa ne padne ispod ograničenja. Korisnik neće moći da šalje poruke do tog trenutka.
- Ograničenje brzine **poruke od 30 poruka u minutu** primenjuje se na sve SKU-ove. To određuje koliko poruka korisnik može da pošalje sa svog Exchange Online nalogu u navedenom periodu.
- Maksimalan broj primalaca koji su dozvoljeni u poljima **Za, Cc** i Bcc za jednu e-poruku, u svim SKU-ovima, jeste **1000 primalaca.** Da biste prilagodili ovo ograničenje, [idite ovde.](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228)
