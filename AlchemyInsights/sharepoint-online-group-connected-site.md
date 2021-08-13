---
title: Dodavanje grupe na SharePoint lokaciju
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200004"
- "5766"
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 52f3bca7e92e9523838b5ad691f8accf0e7d0d03df79bb575f93b024e32cf3c4
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "54093726"
---
# <a name="common-issues-when-creating-a-group-connected-site-in-sharepoint"></a>Uobičajeni problemi prilikom pravljenja sajta povezane sa grupom u SharePoint

1. Ako ste izbrisali grupu i njen povezani sajt i želite da kreirate još jedan sajt sa istim URL adresom, trebalo bi da trajno uklonite prethodni sajt.

   - Preuzimanje [alatke SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)
   - Više informacija o prvim koracima uz PowerShell potražite u članku Prvi [koraci u programu SharePoint Online Management Shell.](/powershell/module/sharepoint-online/remove-sposite)
   - Uklonite lokaciju sa izbrisanih sajtova pomoću [Remove-SPODeletedSite](/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Powershell cmdlet. PowerShell je neophodan za trajno brisanje sajtova grupe.

1. Ako kreirate sajt povezan na grupu i dobićete upozorenje: Druga grupa sa istim pseudonimom već postoji , proverite postojeće grupe iz [Microsoft 365 centar administracije.](https://admin.microsoft.com/AdminPortal/Home#/groups) Da biste rešili ovaj problem, izbrišite postojeću grupu ako vam više nije potrebna ili kreirajte lokaciju sa drugim dodeljenim pseudonimom.

1. Postoje različiti načini za pravljenje i korišćenje modernih grupa pomoću SharePoint.

   - Postojeće sajtove možete povezati sa Microsoft 365 grupama. Dodatne informacije potražite [u Povezivanje grupe Microsoft 365 korišćenjem SharePoint korisničkog interfejsa.](/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface)
   - Da biste kreirali Microsoft 365 povezanu lokaciju grupe, potrebno je da kreirate [lokaciju tima.](https://admin.microsoft.com/sharepoint)
