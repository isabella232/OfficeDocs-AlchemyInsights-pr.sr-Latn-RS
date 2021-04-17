---
title: Obaveštenja u usluzi Yammer
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
- "9002878"
- "5480"
ms.openlocfilehash: 8e7c03f2b557a7d3c409b2ee418df055d0569ee6
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833593"
---
# <a name="notifications-in-yammer"></a>Obaveštenja u usluzi Yammer

Da biste vas obavestila o novoj aktivnosti u relevantnim razgovorima, [usluga Yammer šalje obaveštenja](https://support.microsoft.com/en-gb/office/enable-or-disable-yammer-email-and-phone-notifications-93e530e0-189f-4768-8f28-7683d48cc996) putem e-pošte ili – ako koristite Yammer na mobilnom uređaju – putem prosleđenih obaveštenja. Yammer vam podrazumevano šalje obaveštenja o mnogim tipovima aktivnosti na mreži. Korisnici mogu da ažuriraju postavke e-pošte preko Yammer veb lokacije a prosleđena obaveštenja se konfigurišu putem aplikacije za mobilne uređaje. 

Yammer je dodao podršku za [interaktivne e-poruke u programu Outlook](https://techcommunity.microsoft.com/t5/outlook-blog/interactive-yammer-emails-in-outlook-on-the-web-are-here/ba-p/1209420). Neke e-poruke (kopija poruke) postaće interaktivne u programu Outlook na vebu. Buduća ispravka će ovu funkciju dodati u druge verzije programa Outlook.

**Tipovi obaveštenja u usluzi Yammer**

- E-poruke (najnovije informacije iz grupe, neko vas poziva u grupu, dobijate poruku u prijemnom poštanskom sandučetu itd.)
- Prosleđena obaveštenja (poslato mobilnim uređajima kada ste pomenuti, primite poruku u prijemnom poštanskom sandučetu itd.)
- Iskačuće stavke za stone računare (kada imate instaliranu Yammer aplikaciju za stone računare, ona korisnicima prikazuje „izlazeća” obaveštenja.)
- Zvono obaveštenja (unutar Yammer veb lokacije, korisnici će videti obaveštenja za različite događaje. Ova obaveštenja ne moraju uvek da imaju pridruženu e-poruku ili prosleđeno obaveštenje.)

Dostupne su [detaljnije informacije o obaveštenjima](https://support.microsoft.com/en-gb/office/enable-or-disable-yammer-email-and-phone-notifications-93e530e0-189f-4768-8f28-7683d48cc996).

**Upravljanje obaveštenjima**

Korisnici moraju da upravljaju sopstvenim obaveštenjima. Dostupne su informacije o tome [kako da omogućite i onemogućite Yammer e-poštu i obaveštenja za mobilne uređaje](https://support.microsoft.com/en-gb/office/enable-or-disable-yammer-email-and-phone-notifications-93e530e0-189f-4768-8f28-7683d48cc996). 

Administratori ne mogu da onemoguće sva obaveštenja ili kontrolišu obaveštenja u ime korisnika. Administratori mogu da [kontrolišu logotip uključen u e-poruke i da li korisnici treba da potvrde poruke](https://docs.microsoft.com/yammer/configure-your-yammer-network/configure-email-and-yammer) objavljene putem e-pošte.

**Obaveštenja e-pošte koja se šalju mnogim korisnicima u organizaciji**

Yammer ponekad pošalje samo jedno obaveštenje e-poštom, a primi ga više korisnika nego što je očekivano. Ovo se dešava kada se lista distribucije, ili neki drugo tip ne-pojedinačnih adresa e-pošte doda u Yammer. Yammer ne zna u svim slučajevima da li se radi o adresi e-pošte koja pripada jednom korisniku ili o adresi koja će uzrokovati da jedna poruka e-pošte bude dostavljena mnogim primaocima. Kada se ovaj problem pojavi, morate da preduzmete mere da biste [suspendovali (deaktivirali) nevažećeg korisnika sa tom adresom e-pošte](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users) u usluzi Yammer. 

Da biste smanjili izglede da dođe do ovog problema, trebalo bi da uradite sledeće:

1. [Nametanje Office 365 identiteta](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity) za Yammer.
2. Sprečite spoljne pošiljaoce da šalju e-poštu u vašu organizaciju ili ograničite pošiljaoce pomoću liste odobrenih naloga.

Ako dođe do ovog problema:

1. Identifikujete primaoca e-poruke koja bi trebalo da se poklapa sa korisnikom u usluzi Yammer. Na primer, all-in-sales@fabrikam.com je lista distribucije za sve ljude u prodaji. Ova lista distribucije bi mogla da se identifikujete iz Yammer e-pošte koju su korisnici primili.
2. Koristite funkciju [deaktiviranja (suspendovanja) u administratoru mreže](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users) da biste suspendovali korisnika koji ima adresu e-pošte all-in-sales@fabrikam.com. Suspenzija može da se poništi, tako da je sigurnija od brisanja. Brisanje korisnika će se dogoditi automatski posle 90 dana.
3. Po potrebi, pregledajte [Izvoz korisnika](https://docs.microsoft.com/yammer/manage-security-and-compliance/export-yammer-enterprise-data#ExportUsers) da biste odredili druge nekorisničke adrese e-pošte koje treba suspendovati.
