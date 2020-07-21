---
title: Više korisnika ne vidi programske dodatke u programu Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.openlocfilehash: 18d3fa535a88af18d8c4b02a5371d0a81c8d28c0
ms.sourcegitcommit: a05276bd623466ad211e1f8d9f0c616672dd3640
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 07/16/2020
ms.locfileid: "45198240"
---
# <a name="multiple-users-not-seeing-add-ins-in-outlook"></a>Više korisnika ne vidi programske dodatke u programu Outlook

Ako testirate Outlook programske dodatke i ako se ništa ne prikaže, kao prvi korak za rešavanje problema, upotrebite funkciju " **Preuzmi konfiguraciju config** PowerShell" da biste proverili da li je parametar za _Appsforofficeenabled omogućen_ . Ako upit vraća vrednost **FALSE**, podesite ovaj parametar tako da koristi **Set-organizationconfig** cmdtime, tako da se programski dodaci **pojavljuju na očekivani** način.

Ne preporučujemo da parametar " _Appsforofficesa_ " je postavljen na **vrednost FALSE**. Vrednost **FALSE** zamenjuje sve gorenavedene postavke administrativne i korisničke uloge i sprečava aktiviranje svih novih aplikacija u organizaciji.

Više informacija potražite u članku [Određivanje administratora i korisnika koji mogu da instaliraju i upravljaju programskim dodacima za Outlook](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins#user-roles).