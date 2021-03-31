---
title: 126 Nije moguće pronaći grešku Pribavljanje poštanskog sandučeta u programu OWA?
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "126"
- "1600020"
ms.assetid: e85bffec-e5ad-418a-8561-dab6257e1864
ms.openlocfilehash: 6bab821aaa3b50c365ef5d25a61bca195c76d7ce
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/30/2021
ms.locfileid: "51426676"
---
# <a name="getting-a-mailbox-not-found-error-in-outlook-on-the-web"></a>Dobijate grešku "Nije pronađeno poštansko sanduče" u programu Outlook na vebu?

Ako koristite Outlook na vebu i  ne možete da dobijete grešku u Poštanskom sandučetu, nalog koji ste koristili za povezivanje sa programom Outlook na vebu nema Exchange Online licencu i zbog toga nijedno poštansko sanduče nije povezano sa nalogom. Vaš administart može da dodeli licencu vašem nalogu tako što će pratiti ove korake:

1. Otvorite [Microsoft 365](https://portal.office.com/adminportal/home#/homepage) centar za administaciju i idite na stavku Aktivni korisnici u odeljku Korisnici i izaberite korisnika koji vidite grešku.  

2. Na stranici korisnika koja se  otvori, idite na odeljak Licence i aplikacije, izaberite odgovarajuću vrednost lokacije i dodelite licencu koja sadrži Exchange Online (razvijte licencu da biste videli detalje o njoj).  Kada završite, kliknite na dugme **Sačuvaj promene.**

U nekim slučajevima, ako je licenca već dodeljena korisničkom nalogu, uklanjanje i ponovna dodela licence pomaže u rešavanju problema i ispravno je obezbeđena u sistemu: 

- Proverite da li su vaše M365 Exchange Online (i druge, ako ih imate) aktuelne i da nisu nedavno istekle.

Kada se uverite da vam pretplata nije istekla i da je dodeljena važeća licenca korisničkom nalogu, do obezbeđivanje licence može da protekne i do 24 časa, tako da ćete možda morati da sačekate da se problem reši. Dodatne informacije potražite u [članku Dodeljivanje licenci i upravljanje im.](https://docs.microsoft.com/deployoffice/overview-licensing-activation-microsoft-365-apps#assign-and-manage-licenses)