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
ms.openlocfilehash: 4bf7680a422f096401f0a87bccd1b8dd11f4489f882bcc06864e37d6a248438c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "54046118"
---
# <a name="calendar-permissions"></a>Dozvole za kalendar

Korisnici mogu da promene sopstvene dozvole za kalendar Outlook na vebu ili drugim klijentima, ali vi ćete možda morati da istražite i kao Outlook.  
Uz Exchange PowerShell cmdlet će vam pokazati dozvolu za kalendar korisnika:

`Get-MailboxFolderPermission <SMTPAddress>:\Calendar | FT -a`

Da biste videli više informacija, pogledajte sledeće:

- [Get-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/get-mailboxfolderpermission?view=exchange-ps)

- [Set-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/set-mailboxfolderpermission?view=exchange-ps)

- [Add-MailboxFolderPermission](https://office.visualstudio.com/DefaultCollection/MAX/_queries/query/Add-MailboxFolderPermission)

Dozvole za kalendar se koriste u deljenju kalendara da biste videli više informacija o deljenju Outlook kalendara, pogledajte ove članke:

- [Deljenje Outlook kalendara sa drugim osobama](https://support.office.com/article/353ed2c1-3ec5-449d-8c73-6931a0adab88)
- [Deljenje kalendara u programu Outlook na vebu za preduzeća](https://support.office.com/article/7ecef8ae-139c-40d9-bae2-a23977ee58d5)

Da biste rešili probleme sa dozvolom kalendara, [možete da koristite Pomoćnik za podršku i oporavak](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f) kalendara.