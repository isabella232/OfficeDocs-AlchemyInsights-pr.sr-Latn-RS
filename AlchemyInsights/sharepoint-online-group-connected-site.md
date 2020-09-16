---
title: Dodavanje grupe na SharePoint sajt
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
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 9bec2f71465e43e1c3cba038e0e68949672ceb8a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771222"
---
# <a name="issues-when-creating-a-group-connected-site-in-sharepoint"></a>Problemi prilikom kreiranja povezane lokacije grupe u sistemu SharePoint

1. Neki uobičajeni problemi se susreжu prilikom kreiranja ili ponovnog kreiranja povezane lokacijske grupe.
Ako ste izbrisali grupu i njenu povezanu sajt i želite da kreirate drugu sajt sa istim URL adresom, moraćete trajno da uklonite prethodnu stranicu.

   - Preuzmite [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)
   - Više informacija o prvi koraci uz PowerShell potražite u članku [Prvi koraci uz SharePoint online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).
   - Uklonite lokaciju sa izbrisanih lokacija pomoću modula za [Uklanjanje-Spodeletedsites](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) PowerShell cmdlet. PowerShell je potreban za trajno brisanje lokacija grupe.

1. Ako kreirate Veb lokaciju povezanu sa grupom i primite upozorenje: **već postoji druga grupa sa istim pseudonima**, pregledajte postojeće grupe iz [Microsoft 365 centra administracije](https://admin.microsoft.com/AdminPortal/Home#/groups). Da biste rešili problem, izbrišite postojeću grupu ako ona više nije potrebna ili kreirajte sajt sa drugim dodeljenim pseudonima.

1. Postoje različiti načini za kreiranje i korišćenje modernih grupa sa sistemom SharePoint.

   - Postojeće lokacije možete povezati sa Microsoft 365 grupom. Više informacija potražite u članku [povezivanje Microsoft 365 grupe pomoću SharePoint korisničkog interfejsa](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).
   - Da biste kreirali Microsoft 365 povezanu lokaciju, moraćete da kreirate [lokaciju tima](https://admin.microsoft.com/sharepoint).
