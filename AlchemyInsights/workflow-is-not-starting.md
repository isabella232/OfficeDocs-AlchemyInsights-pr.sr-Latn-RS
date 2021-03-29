---
title: Tok posla se ne pokreće
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: e69f3e529e4a2202f641cb62f42b1a20d774a398
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/29/2021
ms.locfileid: "51403757"
---
# <a name="workflow-is-not-starting"></a>Tok posla se ne pokreće

- SharePoint 2010 i SharePoint 2013 tokovi posla se ne počinju.

    - Ako se tok posla ne pokreće, možda postoji privremeni problem sa uslugom gde korisnici mogu imati povremena odlaganja sa tokom toka posla. Proverite [kontrolnu tablu za zdravlje usluge](https://admin.microsoft.com/AdminPortal/Home/servicehealth) da biste videli da li ima uticaja na vašu organizaciju.

    - Ako je prošlo više od 24 časa od kada ste prvi put videli ovaj problem, prijavite tiket za podršku. U mnogim slučajevima već radimo na rešenju. Dajte nam najmanje 24 sata da dovršimo rešenje.

- SharePoint 2010 tokovi posla odloženi pri pokretanju.

    - To se dešava ako se tok posla pokrene u velikim grupama. (Na primer, kada se istovremeno doda nekoliko stavki).

    - Tokovi posla nisu dizajnirani za pokretanje u realnom vremenu, pa je odlaganje ponašanje po dizajnu.

   -  Ako je tok posla složen jezik za naznake extensible Object Markup (XMOL), kompajlacija može biti spora. Pogledajte [ovaj](https://support.microsoft.com//kb/3043697) članak.

    - Trebalo bi da pojednostaviti tok posla ili ga redizajnovati pomoću tipa platforme Microsoft SharePoint 2013 toka posla.

    - Ako je vaša istorija toka posla velika, možda ćete želeti da ih iščistite ili da napravite novu listu istorije.

        Više informacija: [Purge Workflow History](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)


## <a name="related-topics"></a>Сродне теме
Želite da isprobate Microsoft Flow u sistemu SharePoint Online?
- [Kreiranje toka](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint i Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 
