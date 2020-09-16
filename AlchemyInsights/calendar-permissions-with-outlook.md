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
# <a name="calendar-permissions"></a><span data-ttu-id="1b9a6-102">Dozvole za kalendar</span><span class="sxs-lookup"><span data-stu-id="1b9a6-102">Calendar Permissions</span></span>

<span data-ttu-id="1b9a6-103">Korisnici mogu da promene sopstvene dozvole za kalendar u programu Outlook na Vebu ili drugim klijentima, ali i kao administrator koje ćete možda morati da istražujete.</span><span class="sxs-lookup"><span data-stu-id="1b9a6-103">Users can change their own Calendar Permissions with Outlook on the Web or other clients, but as an admin you may need to investigate as well.</span></span>  
<span data-ttu-id="1b9a6-104">Uz Exchange PowerShell cmdlet vam pokazuje dozvolu za kalendar korisnika:</span><span class="sxs-lookup"><span data-stu-id="1b9a6-104">With Exchange PowerShell cmdlet will show you the permission on a user’s calendar:</span></span>

`Get-MailboxFolderPermission <SMTPAddress>:\Calendar | FT -a`

<span data-ttu-id="1b9a6-105">Da biste videli više informacija pogledajte sledeće:</span><span class="sxs-lookup"><span data-stu-id="1b9a6-105">To see more information see the following:</span></span>

- [<span data-ttu-id="1b9a6-106">Nabavite-Mailboxfolderaccess</span><span class="sxs-lookup"><span data-stu-id="1b9a6-106">Get-MailboxFolderPermission</span></span>](https://docs.microsoft.com/powershell/module/exchange/get-mailboxfolderpermission?view=exchange-ps)

- [<span data-ttu-id="1b9a6-107">Komplet-Mailboxfolderaccess</span><span class="sxs-lookup"><span data-stu-id="1b9a6-107">Set-MailboxFolderPermission</span></span>](https://docs.microsoft.com/powershell/module/exchange/set-mailboxfolderpermission?view=exchange-ps)

- [<span data-ttu-id="1b9a6-108">Programski dodatak Add-mailboxfolder</span><span class="sxs-lookup"><span data-stu-id="1b9a6-108">Add-MailboxFolderPermission</span></span>](https://office.visualstudio.com/DefaultCollection/MAX/_queries/query/Add-MailboxFolderPermission)

<span data-ttu-id="1b9a6-109">Dozvole kalendara se koriste u deljenju kalendara da biste videli više informacija o deljenju Outlook kalendara, pogledajte ove članke:</span><span class="sxs-lookup"><span data-stu-id="1b9a6-109">Calendar Permissions are used in the sharing of calendars, to see more information about sharing an Outlook calendar, see these articles:</span></span>

- [<span data-ttu-id="1b9a6-110">Deljenje Outlook kalendara sa drugim osobama</span><span class="sxs-lookup"><span data-stu-id="1b9a6-110">Share an Outlook calendar with other people</span></span>](https://support.office.com/article/353ed2c1-3ec5-449d-8c73-6931a0adab88)
- [<span data-ttu-id="1b9a6-111">Deljenje kalendara u programu Outlook na vebu za preduzeća</span><span class="sxs-lookup"><span data-stu-id="1b9a6-111">Share your calendar in Outlook on the web for business</span></span>](https://support.office.com/article/7ecef8ae-139c-40d9-bae2-a23977ee58d5)

<span data-ttu-id="1b9a6-112">Da biste rešili problem sa kalendarom, možete da koristite alatku [Pomoćnik za podršku i oporavak](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f) .</span><span class="sxs-lookup"><span data-stu-id="1b9a6-112">To troubleshoot Calendar Permission you can use the [Support and Recovery Assistant](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f) tool.</span></span>