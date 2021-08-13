---
title: Promena podrazumevanog Yammer domena
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
- "9002662"
- "5162"
ms.openlocfilehash: dd29f2dc044fe4ee7f50acc6f0ca491d0ceb80bc360534de10d4010230614f80
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "53950130"
---
# <a name="changing-the-defaultprimary-yammer-domain"></a>Promena podrazumevanog/primarnog Yammer domena

Yammer URL sadrži trenutno primarno ime domena za Yammer mrežu. Ovo ime domena se možda ne poklapa sa primarnim domenom postavljenim u sistemu Office 365 ili Azure AD. Postoje razlike u ponašanju na osnovu broja prilagođenih domena koji su dodati zakupcu, kao i da li je Yammer u podržanoj konfiguraciji (1 zakupac: 1 mreža, ili 1:1). Dokumentacija o [Yammer domenima i Office 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/manage-yammer-domains) je dostupna.

Najčešći razlog zašto vidite neispravan domen je postojanje više Yammer mreža koje treba da se konsoliduju. [Konsolidovanje naniže na pojedinačnu mrežu ](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks) korišćenjem alatke za migraciju mreže predstavlja važan prvi korak. Dovršite ovo pre pokušaja podešavanja primarnog domena.

**Bez prilagođenih domena**

Za nove zakupce, podrazumevani domen (npr. fabrikam.onmicrosoft.com) od zakupca će se koristiti za Yammer. Primarni domen je postavljen na yammer.com/fabrikam.onmicrosoft.com.

**Pojedinačni prilagođeni domen**

Yammer će automatski izabrati prilagođeni domen (npr. fabrikam.com) od zakupca kao primarni domen u usluzi Yammer. Podešeno je na yammer.com/fabrikam.com. Ova promena je napravljena od strane usluge sinhroniziranja domena i može da potraje do 24 časa da bi stupila na snagu.

**Višestruki prilagođeni domeni**

Yammer može da ima primarni domen koji se razlikuje od podrazumevanog domena zakupca. Budući da postoji više prilagođenih domena, Yammer ne pokušava da pogodi tačan, dostupan domen. Morate da otvorite predmet podrške da biste zahtevali da se primarni naziv domena promeni u primarni domen po vašem izboru.

**Dodatne informacije o rešavanju problema**

U nekim slučajevima domeni su možda premešteni između zakupaca i usluga sinhronizacije domena nije mogla uspešno da se pokrene. Možete iskusiti problem sa prijavljivanjem ili druge probleme, pored netačnog primarnog domena. Da biste rešili ovaj problem, domeni će možda morati da se premeste u ispravnu mrežu uz pomoć Microsoft podrške. Ova situacija zahteva direktnu pomoć i rešenje može da potraje neko vreme, posebno ako postoji dugačka lista imena domena. Otvorite predmet podrške da biste dobili pomoć za rešavanje ove vrste problema.

Radeći sa agentom za podršku, oni će proveriti da li su se domeni verifikovani kod zakupca pod vašom kontrolom. Oni mogu da postavljaju dodatna pitanja za verifikaciju u vezi sa domenima ako se dodaju vašem zakupcu, ali nisu verifikovani od strane DNS. Molimo obezbedite da su domeni verifikovani od strane DNS-a da biste ubrzao proces.
