---
title: Endpoint Manager – odrednice bezbednosti
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10084"
- "6700005"
- "10064"
- "9003771"
ms.openlocfilehash: 36b480c7ed4715338fda056eafd69c511093e627
ms.sourcegitcommit: bef118c00aa397cd6d8941d403fe9cfa49dd8c73
ms.translationtype: HT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/30/2021
ms.locfileid: "51440907"
---
# <a name="endpoint-manager---security-baselines"></a>Endpoint Manager – odrednice bezbednosti

Osnovne informacije o bezbednosti su unapred konfigurisane grupe postavki operativnog sistema Windows koje vam pomažu da primenite bezbednosne postavke koje preporučuju relevantni bezbednosni timovi. Ove odrednice mogu da se prilagode tako da isporuče samo postavke i vrednosti koje želite. Više informacija o osnovnim informacijama o bezbednosti pogledajte u [Korišćenje osnovnih podataka o bezbednosti za konfigurisanje Windows 10 uređaja u Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines).

Trenutno postoje odrednice za ove proizvode:

- Windows MDM bezbednosne postavke
- Microsoft zaštitnik za EndPoint bezbednost
- Microsoft Edge

Svaka odrednica se periodično ažurira i objavljuje u inkrementalnim verzijama. Svaka verzija dodaje ili uklanja postavke iz prethodne verzije kako bi se obezbedilo da odrednica ispunjava trenutna uputstva. Konzola odrednica sigurnosti u programu Endpoint bezbednost omogućava upoređivanje različitih verzija čineći promene iz verzije u verziju vidljivim.

Uputstvo o tome kako da na najefikasniji način promenite koja se verzija odrednica primenjuje možete da vidite u članku [Upravljanje osnovnim profilima bezbednosti u aplikaciji Microsoft Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure).

Nakon primene odrednica bezbednosti možete da pratite stanje primene i pregledate postavke od uređaja do uređaja.

**Namena:** podaci o izveštavanju za odrednice mogu potrajati i do 24 sata da se pojave od početne primene na uređaju i do 6 sati za dalja ažuriranja. 

Najčešći uzrok postavke odrednice koja se ne primenjuje jeste zato što se ista postavka koristi na drugom profilu. Ovaj scenario se može istražiti za određeni uređaj tako što će izabrati taj uređaj u okviru statusa uređaja u okviru profila bezbednosne odrednice. Detalje možete da vidite u [Rešavanje neusaglašenosti za bezbednosne odrednice](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines).