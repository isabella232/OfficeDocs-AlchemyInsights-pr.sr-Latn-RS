---
title: Dozvole za kalendar
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3800009"
- "611"
ms.openlocfilehash: bbd49134bd4a4451649b76bb5f60b19065910cae
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819922"
---
# <a name="calendar-permissions"></a>Dozvole za kalendar

Korisnici mogu da promene svoje dozvole za kalendar uz Outlook na vebu ili druge klijente, ali vi ćete možda morati da istražite i kao adminimenata.  
Uz Exchange PowerShell cmdlet će vam pokazati dozvolu za kalendar korisnika:

`Get-MailboxFolderPermission <SMTPAddress>:\Calendar | FT -a`

Da biste videli više informacija, pogledajte sledeće:

- [Get-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/get-mailboxfolderpermission?view=exchange-ps)

- [Set-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/set-mailboxfolderpermission?view=exchange-ps)

- [Add-MailboxFolderPermission](https://office.visualstudio.com/DefaultCollection/MAX/_queries/query/Add-MailboxFolderPermission)

Dozvole za kalendar se koriste u deljenju kalendara da biste videli više informacija o deljenju Outlook kalendara, pogledajte ove članke:

- [Deljenje Outlook kalendara sa drugim osobama](https://support.office.com/article/353ed2c1-3ec5-449d-8c73-6931a0adab88)
- [Deljenje kalendara u programu Outlook na vebu za preduzeća](https://support.office.com/article/7ecef8ae-139c-40d9-bae2-a23977ee58d5)

Da biste rešili probleme sa dozvolom za kalendar, možete da [koristite alatku "Pomoćnik za podršku i oporavak".](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f)