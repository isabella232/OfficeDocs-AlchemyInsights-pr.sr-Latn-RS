---
title: SharePoint Problemi sa vezom dizajnera
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
ms.openlocfilehash: d55f7c1902bb623900fa74bdae70695b6e04ad84ce7b6ea314db614283ec436d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "53942039"
---
# <a name="sharepoint-designer-connection-issues"></a>SharePoint Problemi sa vezom dizajnera 

Ako SharePoint Problema sa vezom ka SharePoint lokacijama, isprobajte sledeća uobičajena rešenja.

1. korak: Proverite da li SharePoint Dizajner 2013 ažurira ispravkom [za SharePoint Designer](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) servisni paket 1 i ispravku od 2. avgusta [2016. za SharePoint Designer 2013.](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721)



2. korak: Brisanje lokalnih datoteka keša:

1. Zatvorite SharePoint Designer 2013.

2. Na lokalnom računaru uklonite sve datoteke pronađene u svakoj od sledećih fascikli.

    - %APPDATA%\Microsoft\Web Server Extensions\Cache
    - %APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache
    - %USERPROFILE%\AppData\Local\Microsoft\WebsiteCache

3. Otvorite SharePoint Designer 2013 i ponovo unesite nalog da biste videli da li radi.

3. korak: [Omogućavanje moderne potvrde identiteta za Kancelarija 2013 na Windows uređajima.](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication)

4. korak: Administratori  će morati da dozvole prilagođenu skriptu u postavkama SharePoint centra administracije da bi omogućili SharePoint dizajnera programa SharePoint. Više [informacija potražite u temi Dozvoljavanje ili sprečavanje prilagođenih](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) skripti.


