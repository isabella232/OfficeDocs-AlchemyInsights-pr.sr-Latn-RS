---
title: Problemi sa SharePoint dizajnerskim povezivanjem
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 997ba3de58485d4fe6d24b926c33348378af8cd3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727185"
---
# <a name="sharepoint-designer-connection-issues"></a>Problemi sa SharePoint dizajnerskim povezivanjem 

Ako SharePoint Designer ima problema sa vezom na SharePoint lokacijama, isprobajte sledeća uobičajena rešenja.

1. prvi: proverite da li se SharePoint Designer 2013 ažurira pomoću [usluge SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) i [2 avgusta, 2016 Update za SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).



2.2: Opozovite izbor u lokalnim datotekama keširanja:

1. Zatvorite SharePoint Designer 2013.

2. Na lokalnom računaru uklonite sve datoteke pronađene u svakoj od sledećih fascikli.

    - %AppData%\microsoft\veb server Extensions\keš
    - %APPDATA%\Microsoft\SharePoint Designer\proxyasekeš
    - %USERPROFILE%\appdata\local\microsoft\websitekeš

3. Otvorite SharePoint Designer 2013 i ponovo unesite nalog da biste videli da li radi.

Treći broj: [omogućite modernu potvrdu identiteta za Office 2013 na Windows uređajima](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).

4. broj: administratori treba da **dozvole prilagođenu tekst** u postavkama sistema SharePoint centra administracije da bi se dozvolila Povezivanje SharePoint dizajnera. Više informacija potražite u članku [Omogućavanje ili sprečavanje prilagođenog skriptova](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) .


