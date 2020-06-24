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
# <a name="calendar-permissions"></a><span data-ttu-id="c3f1b-102">Dozvole za kalendar</span><span class="sxs-lookup"><span data-stu-id="c3f1b-102">Calendar Permissions</span></span>

<span data-ttu-id="c3f1b-103">Korisnici mogu da promene sopstvene dozvole kalendara sa programom Outlook na Vebu ili drugim klijentima, ali kao administrator će možda morati i da istraži.</span><span class="sxs-lookup"><span data-stu-id="c3f1b-103">Users can change their own Calendar Permissions with Outlook on the Web or other clients, but as an admin you may need to investigate as well.</span></span>  
<span data-ttu-id="c3f1b-104">Sa Exchange PowerShell cmdmo će vam pokazati dozvolu za korisnički kalendar:</span><span class="sxs-lookup"><span data-stu-id="c3f1b-104">With Exchange PowerShell cmdlet will show you the permission on a user’s calendar:</span></span>

`Get-MailboxFolderPermission <SMTPAddress>:\Calendar | FT -a`

<span data-ttu-id="c3f1b-105">Da biste videli više informacija pogledajte sledeće:</span><span class="sxs-lookup"><span data-stu-id="c3f1b-105">To see more information see the following:</span></span>

- [<span data-ttu-id="c3f1b-106">Get-MailboxFolderPermission</span><span class="sxs-lookup"><span data-stu-id="c3f1b-106">Get-MailboxFolderPermission</span></span>](https://docs.microsoft.com/powershell/module/exchange/get-mailboxfolderpermission?view=exchange-ps)

- [<span data-ttu-id="c3f1b-107">Set-MailboxFolderPermission</span><span class="sxs-lookup"><span data-stu-id="c3f1b-107">Set-MailboxFolderPermission</span></span>](https://docs.microsoft.com/powershell/module/exchange/set-mailboxfolderpermission?view=exchange-ps)

- [<span data-ttu-id="c3f1b-108">Add-MailboxFolderPermission</span><span class="sxs-lookup"><span data-stu-id="c3f1b-108">Add-MailboxFolderPermission</span></span>](https://office.visualstudio.com/DefaultCollection/MAX/_queries/query/Add-MailboxFolderPermission)

<span data-ttu-id="c3f1b-109">Dozvole za kalendar se koriste u deljenju kalendara, da biste videli više informacija o deljenju Outlook kalendara, pogledajte sledeće članke:</span><span class="sxs-lookup"><span data-stu-id="c3f1b-109">Calendar Permissions are used in the sharing of calendars, to see more information about sharing an Outlook calendar, see these articles:</span></span>

- [<span data-ttu-id="c3f1b-110">Deljenje Outlook kalendara sa drugim osobama</span><span class="sxs-lookup"><span data-stu-id="c3f1b-110">Share an Outlook calendar with other people</span></span>](https://support.office.com/article/353ed2c1-3ec5-449d-8c73-6931a0adab88)
- [<span data-ttu-id="c3f1b-111">Deljenje kalendara u programu Outlook na Webu za posao</span><span class="sxs-lookup"><span data-stu-id="c3f1b-111">Share your calendar in Outlook on the web for business</span></span>](https://support.office.com/article/7ecef8ae-139c-40d9-bae2-a23977ee58d5)

<span data-ttu-id="c3f1b-112">Da biste rešili problem sa dozvolom kalendara, možete da koristite alatku " [Pomoćnik za podršku i oporavak](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f) ".</span><span class="sxs-lookup"><span data-stu-id="c3f1b-112">To troubleshoot Calendar Permission you can use the [Support and Recovery Assistant](https://support.microsoft.com/office/e90bb691-c2a7-4697-a94f-88836856c72f) tool.</span></span>