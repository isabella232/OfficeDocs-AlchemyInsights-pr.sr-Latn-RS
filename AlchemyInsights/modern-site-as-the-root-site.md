---
title: Moderni sajt kao osnovni sajt
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
ms.openlocfilehash: a0f48dc79b51168c9cc045078ad8fc7d668343c7
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/13/2021
ms.locfileid: "58327616"
---
# <a name="modern-site-as-root-site"></a>Moderni sajt kao osnovni sajt

Počeli smo sa unošenjem nove funkcije koja će vam omogućiti da zamenite klasični osnovni [sajt sajta sa modernim sajtom.](https://docs.microsoft.com/sharepoint/modern-root-site) Koristite [invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) da biste zamenili lokaciju lokacije sa drugim sajtom prilikom arhiviranje originalnog sajta. Dostupno za sajt tima (nije povezan sa grupom) i sajtu za komunikaciju.

**Važno:** Nemojte brisati klasični osnovni sajt da biste kreirali moderan sajt za komunikaciju. Microsoft to ne podržava. Brisanjem osnovne lokacije sve SharePoint u organizaciji neće biti dostupne svim korisnicima, sve dok ne vratite lokaciju u prethodno stanje ili kreirate novi sajt na istom URL adresi. Ovu funkciju ćemo preneti putem centra za poruke. Trebalo bi da očekujete da ta funkcija bude uskoro uključena u zakučaru.

## <a name="known-issues-with-swapping-sites"></a>Poznati problemi sa zamenom sajtova
- Ciljni sajt može dati grešku "nije pronađeno" (HTTP 404) tokom kratkog vremenskog perioda.
- Sadržaj treba ponovo da se pretražuje da bi se ažurirao indeks za pretraživanje. Ovde ne postoji ručni korak, ovo će biti automatski urađeno.
- Sve što zavisi od "statičnih" veza (kao što su sinhronizacija datoteka i OneNote datoteke) moraće ručno da se ispravi.
- Project Možda će biti potrebno proveriti valjanost lokacija servera da biste se uverili da su i dalje ispravno povezane. 
