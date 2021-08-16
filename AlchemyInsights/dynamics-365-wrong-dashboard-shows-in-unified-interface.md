---
title: Dynamics 365 – Pogrešna kontrolna tabla prikazuje se u Dynamics 365 unifikovanom interfejsu
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
ms.openlocfilehash: 1edb2a7e9e0c270c7e98eb43d2f6514d70c39a19ea97d189322ca387b6842a18
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "54101496"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a>Pogrešna kontrolna tabla prikazuje se u Dynamics 365 unifikovanom interfejsu

Postoji nekoliko razloga zbog kojih možete da vidite drugačiju tablu od one koja je očekivana:

## <a name="the-user-has-set-a-user-default-dashboard"></a>Korisnik je postavio podrazumevanu dashboard korisnika 

Obično možete da identifikujete podrazumevanu korisničku dashboard is set if the **Set As Default button** does not show in the dashboard command bar. Korisnička podrazumevana dashboard će poništiti sve druge podrazumevane komandne table, čak i ako podrazumevana komandna tabla korisnika nije u trenutnoj aplikaciji.

Koristite sledeće zaostavnje da biste poništili njihovu podrazumevanu dasku.

1. Kreirajte novu ličnu dashboard.

2. Postavite tu novu dashboard kao podrazumevanu korisnika.

3. Izbrišite tu dashboard.

## <a name="the-dashboard-is-set-in-the-sitemap"></a>Dashboard is set in the sitemap

Možda ste podesili podrazumevanu e-tablu organizacije tako što ste izabrali stavku "Šta treba da se koristi" i odabrati stavku "Postavi kao podrazumevano" u okviru stavke "Prilagođavanje sistema". Međutim, što je definisano u dizajneru mape sajta, imaće prestst u vezi sa ovom dashboard, ako korisnik ima pristup.

Da bi korisnici videli tablu koje ste postavili kao podrazumevanu organizaciju, možete:

* Postavljanje te dashboard in the sitemap

* Uklanjanje pristupa definisanoj tabli mape sajta za te korisnike
