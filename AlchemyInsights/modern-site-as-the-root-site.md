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
ms.openlocfilehash: b42cf276a76547584c8cfd87b5a28f31d51ea7f8ca56621b22aeef01e4613ce6
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "54000406"
---
# <a name="modern-site-as-root-site"></a>Moderni sajt kao osnovni sajt

Počeli smo sa unošenjem nove funkcije koja će vam omogućiti da zamenite klasični osnovni [sajt sa modernim sajtom.](https://docs.microsoft.com/sharepoint/modern-root-site) Koristite [invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) da biste zamenili lokaciju lokacije sa drugim sajtom prilikom arhiviranje originalnog sajta. Dostupno za sajt tima (nije povezan sa grupom) i sajtu za komunikaciju.

>[!Important]
> Nemojte brisati klasični osnovni sajt da biste kreirali moderni sajt za komunikaciju. Microsoft to ne podržava. Brisanjem osnovne lokacije sve SharePoint u organizaciji neće biti dostupne svim korisnicima dok je ne vratite u prethodno stanje ili ne kreirate novi sajt na istom URL adresi. Ovu funkciju ćemo preneti putem centra za poruke. Trebalo bi da očekujete da ta funkcija bude uskoro uključena u zakučaru.

## <a name="known-issues-with-swapping-sites"></a>Poznati problemi sa zamenom sajtova
- Ciljni sajt može dati grešku "nije pronađeno" (HTTP 404) tokom kratkog vremenskog perioda.
- Sadržaj treba ponovo da se pretražuje da bi se ažurirao indeks za pretraživanje. Ovde ne postoji ručni korak, ovo će biti automatski urađeno.
- Sve što zavisi od "statičnih" veza (kao što su sinhronizacija datoteka i OneNote datoteke) moraće ručno da se ispravi.
- Project Možda će biti potrebno proveriti valjanost lokacija servera da biste se uverili da su i dalje ispravno povezani. 
