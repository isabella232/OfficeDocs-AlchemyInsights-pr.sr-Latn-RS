---
title: Moderna lokacija kao osnovna lokacija
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ms.date: 04/21/2020
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: 86ff5f7fbaed62de9047006bf4ba4d2db2be3def
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47666884"
---
# <a name="modern-site-as-root-site"></a>Savremena lokacija kao osnovna lokacija

Počeli smo da ovodimo novu funkciju koja će vam omogućiti da [zamenite klasičnu osnovnu veb sajt sajta modernom lokacijom](https://docs.microsoft.com/sharepoint/modern-root-site). Korišćenje poziva [-Spositesvp](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) za razmenu lokacije sa drugom lokacijom dok arhivirate originalnu lokaciju. Dostupno za oba sajta tima (nije povezano sa grupom) i sajt za komunikaciju.

>[!Important]
> Nemojte da izbrišete klasičnu osnovnu sajt da biste kreirali modernu sajt za komunikaciju. Microsoft ne podržava ovo. Brisanje osnovne lokacije će učiniti da sve SharePoint lokacije u vašoj organizaciji budu nedostupne svim korisnicima dok ne vratite lokaciju ili kreirate novu lokaciju na istoj URL adresi. Ovu funkciju ćemo komunicirati putem centra za poruke. Trebalo bi da očekujete da će funkcija uskoro biti uključena u zakupca.

## <a name="known-issues-with-swapping-sites"></a>Poznati problemi sa Veb lokacijama
- Ciljna lokacija može da vrati grešku "nije pronađena" (HTTP 404) na kratko vreme.
- Potrebno je ponovo popisivati sadržaj da biste ažurirali indeks pretrage. Ovde ne postoji potreban ručni korake, ovo će biti gotovo automatski.
- Sve što zavisi od veza "statične" (kao što su sinhronizacija datoteka i OneNote datoteke) mora se ručno ispraviti.
- Za lokacije servera projekta možda će biti potrebno da se verifikujete da biste se uverili da su i dalje ispravno povezane. 
