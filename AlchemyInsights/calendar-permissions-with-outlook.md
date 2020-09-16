---
title: Dozvole za kalendar
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3800009"
- "611"
ms.openlocfilehash: cfee520e26587c0a649c08084853c31232d027f8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47748807"
---
# <a name="calendar-permissions"></a>Dozvole za kalendar

Korisnici mogu da promene sopstvene dozvole za kalendar u programu Outlook na Vebu ili drugim klijentima, ali i kao administrator koje ćete možda morati da istražujete.  
Uz Exchange PowerShell cmdlet vam pokazuje dozvolu za kalendar korisnika:

`Get-MailboxFolderPermission <SMTPAddress>:\Calendar | FT -a`

Da biste videli više informacija pogledajte sledeće:

- [Nabavite-Mailboxfolderaccess](https://docs.microsoft.com/powershell/module/exchange/get-mailboxfolderpermission?view=exchange-ps)

- [Komplet-Mailboxfolderaccess](https://docs.microsoft.com/powershell/module/exchange/set-mailboxfolderpermission?view=exchange-ps)

- [Programski dodatak Add-mailboxfolder](https://office.visualstudio.com/DefaultCollection/MAX/_queries/query/Add-MailboxFolderPermission)

Dozvole kalendara se koriste u deljenju kalendara da biste videli više informacija o deljenju Outlook kalendara, pogledajte ove članke:

- [Deljenje Outlook kalendara sa drugim osobama](https://support.office.com/article/353ed2c1-3ec5-449d-8c73-6931a0adab88)
- [Deljenje kalendara u programu Outlook na vebu za preduzeća](https://support.office.com/article/7ecef8ae-139c-40d9-bae2-a23977ee58d5)

Da biste rešili problem sa kalendarom, možete da koristite alatku [Pomoćnik za podršku i oporavak](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f) .