---
title: Dynamics 365-pogrešan instrument Kontrolna tabla u programu Dynamics 365 objedinjeno interfejs
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1484"
- "6200024"
ms.openlocfilehash: 02e33c7dbdfe9b7d2ad7a04f154cf067fba0aab2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47711289"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a>Pogrešna Kontrolna tabla prikazuje u dinamici Dynamics 365

Postoji nekoliko razloga zbog kojih možete da vidite drugu kontrolnu tablu od one koju očekujete:

## <a name="the-user-has-set-a-user-default-dashboard"></a>Korisnik je podesio podrazumevani instrument-tablu 

Najčešće možete identifikovati korisničku početnu kontrolnu tablu ako se dugme **Postavi kao podrazumevano** ne prikaže na komandnoj traci kontrolne table. Kontrolna tabla korisnika će zameniti sve druge podrazumevane kontrolne table, čak i ako podrazumevana Kontrolna tabla korisnika nije u trenutnoj aplikaciji.

Koristite sledeće zaobilaženje problema da biste osmestili podrazumevanu kontrolnu tablu.

1. Kreirajte novu ličnu tablu.

2. Postavi tu novu kontrolnu tablu kao podrazumevanu vrednost korisnika.

3. Izbrišite tu kontrolnu tablu.

## <a name="the-dashboard-is-set-in-the-sitemap"></a>Kontrolna tabla je postavljena na mapi sajta

Možda ste odredili početnu kontrolnu tablu organizacije tako što ćete izabrati kontrolnu tablu i izabrati stavku "Postavi kao podrazumevano" u okviru "Prilagođavanje sistema". Međutim, Kontrolna tabla koja je definisana u dizajneru "sajt" će imati prvenstvo iznad ove kontrolne table ako korisnik ima pristup.

Da bi korisnici videli kontrolnu tablu koju ste odredili kao podrazumevanu organizaciju, možete da:

* Podesite kontrolnu tablu na mapi sajta

* Uklanjanje pristupa definisanoj kontrolnoj tabli za te korisnike
