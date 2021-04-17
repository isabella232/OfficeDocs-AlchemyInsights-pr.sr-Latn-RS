---
title: Kompatibilnost aplikacija sa aplikacijom Microsoft Surface Pro X
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/14/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7009"
- "9003951"
ms.openlocfilehash: 085815982a3948a7853326541101d2ed21c1869e
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/15/2021
ms.locfileid: "51837419"
---
# <a name="app-compatibility-with-microsoft-surface-pro-x"></a>Kompatibilnost aplikacija sa aplikacijom Microsoft Surface Pro X

Aplikacije se različito pokrećaju na uređajima kao što je Surface Pro X. Većina aplikacija je kompatibilna, ali postoje neka ograničenja. Evo liste problema koje možete imati prilikom pokretanje aplikacije: 

**Upravljački programi.** Upravljački programi će raditi ako su dizajnirani za računar zasnovan na ARM operativnom sistemu Windows 10. Ako upravljački program ne radi, aplikacija ili hardver na koji se oslanja neće raditi. Dodatnu podršku za uređaj možete da pogledate u najčešćim temama o računarima zasnovanim na ARM operativnom sistemu [Windows 10](https://support.microsoft.com/windows/windows-10-arm-based-pcs-faq-477f51df-2e3b-f68f-31b0-06f5e4f8ebb5) ili se obratite proizvođaču hardvera.

**64-bitne (x64) aplikacije.** Aplikacije koje su 64-bitne (x64) neće raditi. Biće vam potrebne 64-bitne (ARM64) aplikacije, 32-bitne (ARM32) aplikacije ili 32-bitne (x86) aplikacije. Obično možete da pronađete 32-bitne (x86) verzije aplikacija, ali neki projektanti aplikacija nude samo 64-bitne (x64) aplikacije.

**Prilagođene aplikacije.** Aplikacije koje prilagođavaju iskustvo pri radu sa operativnim sistemom Windows, kao što su pomoćne tehnologije ili aplikacije za skladištenje u oblaku, mogu naići na probleme. Da biste saznali više, obratite se proizvođaču aplikacije.

**Antivirusni softver nezavisnih proizvođača.** Ne možete da instalirate neki antivirusni softver nezavisnog proizvođača. Windows bezbednost vam pomaže da ostanete bezbedni u toku podržanog veka vašeg Windows 10 uređaja.

**Windows faks i skener.** Windows faks i skener nisu dostupni na računaru zasnovanom na ARM operativnom sistemu Windows 10.

Ako otkrijete da naižete na probleme sa instaliranjem, deinstalijom ili poništavanju aplikacije, pogledajte detalje [o rešavanju problema sa aplikacijom.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-app-install#app-troubleshooting-details)

Osim u retkim slučajevima, sve ključne reči bi trebalo da budu OR umesto AND.