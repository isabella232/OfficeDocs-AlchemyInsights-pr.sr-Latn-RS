---
title: Dodavanje grupe na SharePoint lokaciju
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 5dab9fce935936898927afd55f8f6e9260249157
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 06/05/2020
ms.locfileid: "44582825"
---
# <a name="issues-when-creating-a-group-connected-site-in-sharepoint"></a>Problemi prilikom kreiranja grupe povezane lokacije u sistemu SharePoint

1. Došlo je do nekih uobičajenih problema prilikom kreiranja ili ponovnog kreiranja grupe povezane lokacije.
Ako ste izbrisali grupu i povezanu lokaciju i želite da kreirate drugu lokaciju sa istom URL adresom, moraćete trajno da uklonite prethodnu lokaciju.

   - Preuzimanje [ljuske za upravljanje SPO](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429) -a
   - Više informacija o početku rada sa programom PowerShell potražite u članku [Prvi koraci u usluzi SharePoint Shell Management ljuske](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).
   - Uklonite lokaciju sa izbrisanih lokacija koristeći [stranicu ukloni-Prebrisedshell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) cmdto. PowerShell je potreban za trajno brisanje grupnih lokacija.

1. Ako kreirate grupu povezanu lokaciju i primite upozorenje: **druga grupa sa istim pseudonimom već postoji**, proverite postojeće grupe iz [Microsoft 365 admin Center](https://admin.microsoft.com/AdminPortal/Home#/groups). Da biste rešili problem, izbrišite postojeću grupu ako više nije potrebna ili kreirajte lokaciju sa dodeljenim drugim pseudonimom.

1. Postoje različiti načini za kreiranje i korišćenje modernih grupa sa SharePoint-om.

   - Postojeće lokacije možete da povežete sa Microsoft 365 grupom. Više informacija potražite u članku [povezivanje Microsoft 365 grupe pomoću SharePoint korisničkog interfejsa](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).
   - Da biste kreirali lokaciju koja je povezana sa Microsoft 365 grupom, moraćete da kreirate [lokaciju tima](https://admin.microsoft.com/sharepoint).
