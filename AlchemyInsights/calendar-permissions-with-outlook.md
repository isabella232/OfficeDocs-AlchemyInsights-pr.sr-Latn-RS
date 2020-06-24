---
title: Dozvole za kalendar
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3800009"
- "611"
ms.openlocfilehash: 78f27014c60badc801212177dd455ef2a0de5a9e
ms.sourcegitcommit: 722e9a0ed058cb1eab2dd053be2418b60f7d4aac
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 06/23/2020
ms.locfileid: "44862169"
---
# <a name="calendar-permissions"></a>Dozvole za kalendar

Korisnici mogu da promene sopstvene dozvole kalendara sa programom Outlook na Vebu ili drugim klijentima, ali kao administrator će možda morati i da istraži.  
Sa Exchange PowerShell cmdmo će vam pokazati dozvolu za korisnički kalendar:

`Get-MailboxFolderPermission <SMTPAddress>:\Calendar | FT -a`

Da biste videli više informacija pogledajte sledeće:

- [Get-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/get-mailboxfolderpermission?view=exchange-ps)

- [Set-MailboxFolderPermission](https://docs.microsoft.com/powershell/module/exchange/set-mailboxfolderpermission?view=exchange-ps)

- [Add-MailboxFolderPermission](https://office.visualstudio.com/DefaultCollection/MAX/_queries/query/Add-MailboxFolderPermission)

Dozvole za kalendar se koriste u deljenju kalendara, da biste videli više informacija o deljenju Outlook kalendara, pogledajte sledeće članke:

- [Deljenje Outlook kalendara sa drugim osobama](https://support.office.com/article/353ed2c1-3ec5-449d-8c73-6931a0adab88)
- [Deljenje kalendara u programu Outlook na Webu za posao](https://support.office.com/article/7ecef8ae-139c-40d9-bae2-a23977ee58d5)

Da biste rešili problem sa dozvolom kalendara, možete da koristite alatku " [Pomoćnik za podršku i oporavak](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f) ".