---
title: Dodavanje grupe na SharePoint lokaciji
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
ms.openlocfilehash: 5dd159b8b9e141c2fb448bae5fb624efe1014d7d
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/13/2021
ms.locfileid: "58318138"
---
# <a name="common-issues-when-creating-a-group-connected-site-in-sharepoint"></a>Uobičajeni problemi prilikom pravljenja sajta povezane sa grupom u SharePoint

1. Ako ste izbrisali grupu i njen povezani sajt i želite da kreirate još jedan sajt sa istim URL adresom, trebalo bi da trajno uklonite prethodni sajt.

   - Preuzimanje [alatke SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)
   - Više informacija o prvim koracima uz PowerShell potražite u članku Prvi [koraci u programu SharePoint Online Management Shell.](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite)
   - Uklonite lokaciju sa izbrisanih sajtova pomoću [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Powershell cmdlet. PowerShell je neophodan za trajno brisanje sajtova grupe.

1. Ako kreirate sajt povezan sa grupom i dobićete upozorenje: Druga grupa sa istim pseudonimom već postoji , proverite postojeće grupe sa lokacije [Microsoft 365 centar administracije.](https://admin.microsoft.com/AdminPortal/Home#/groups) Da biste rešili problem, izbrišite postojeću grupu ako vam više nije potrebna ili kreirajte lokaciju sa drugim dodeljenim pseudonimom.

1. Postoje različiti načini za pravljenje i korišćenje modernih grupa pomoću SharePoint.

   - Postojeće sajtove možete povezati sa Microsoft 365 grupama. Više informacija potražite u Povezivanje [grupe Microsoft 365 pomoću SharePoint korisničkog interfejsa.](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface)
   - Da biste kreirali Microsoft 365 povezanu lokaciju grupe, potrebno je da kreirate [lokaciju tima.](https://admin.microsoft.com/sharepoint)
