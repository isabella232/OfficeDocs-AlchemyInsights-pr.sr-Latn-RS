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
ms.openlocfilehash: e3b8777ed74b812b31338784999eea43a95d3456
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/15/2020
ms.locfileid: "47794781"
---
# <a name="workflow-is-not-starting"></a>Tok posla se ne pokreće

- SharePoint 2010 i SharePoint 2013 tokovi posla ne počinju.

    - Ako se tok posla ne pokreće, možda postoji privremeni problem pri uslugama gde korisnici mogu da doživljaju prekida kašnjenja sa napretkom toka posla. Pogledajte [kontrolnu tablu zdrave usluge](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) da biste videli da li je vaša organizacija uticala na njih.

    - Ako je prošlo više od 24 časa od kada ste prvi put videli ovaj problem, prijavite karticu podrške. U mnogim slučajevima, već radimo na rešenju. Dajte nam najmanje 24 časa da biste dovršili rešenje.

- SharePoint 2010 tokovi posla odloženi na početnom meniju.

    - Do ovoga dolazi ako je tok posla izazvan velikim grupama. (na primer, kada se odjednom doda nekoliko stavki).

    - Tokovi posla nisu dizajnirani za pokretanje u realnom vremenu, tako da je kašnjenje po dizajnu dizajn.

   -  Ako je tok posla složen Extensible Object Markup Language (XMOL), kompilacija može biti spora. Potvrdite [ovaj](https://support.microsoft.com//kb/3043697) članak.

    - Trebalo bi da pojednostavite tok posla ili da ga ponovo dizajnirate pomoću programa Microsoft SharePoint 2013 toka posla.

    - Ako je vaša istorija toka posla porasla, možda ćete želeti da očistite stavke ili da kreirate novu listu istorije.

        Više informacija: [Čišćenje istorije toka posla](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)


## <a name="related-topics"></a>Сродне теме
Želite da probate Microsoft flow u usluzi SharePoint online?
- [Kreiranje protoka](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint i protok](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


