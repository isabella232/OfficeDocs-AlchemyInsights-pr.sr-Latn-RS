---
title: Pošiljalac ne prima e-poštu koja se šalje u Microsoft 365 grupi
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/20/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
ms.openlocfilehash: b3b438e17c35f18289d3e9c3ca89d16a6f2a065f
ms.sourcegitcommit: dcca0df53f9194f406cf3a5f6b046cb33a0a5b03
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/21/2020
ms.locfileid: "46872118"
---
# <a name="sender-does-not-receive-email-sent-to-microsoft-365-group"></a><span data-ttu-id="3cd1b-102">Pošiljalac ne prima e-poštu koja se šalje u Microsoft 365 grupi</span><span class="sxs-lookup"><span data-stu-id="3cd1b-102">Sender does not receive email sent to Microsoft 365 group</span></span>

<span data-ttu-id="3cd1b-103">Pošiljalac e-365 poruke podrazumevano ne prima kopiju poruke u prijemnom poštanskom sandučetu, čak i ako je pošiljalac član grupe.</span><span class="sxs-lookup"><span data-stu-id="3cd1b-103">By default, the sender of an email message to a Microsoft 365 group doesn't receive a copy of the message in their Inbox, even if the sender is a member of the group.</span></span>

<span data-ttu-id="3cd1b-104">Koristite ovu komandu EXO PowerShell da biste omogućili pošiljaocu da primi kopiju svake e-poruke koju pošalju u Microsoft 365 grupu:</span><span class="sxs-lookup"><span data-stu-id="3cd1b-104">Use this EXO PowerShell command to allow the sender to receive a copy of each email they send to the Microsoft 365 group:</span></span>  

`Set-MailboxMessageConfiguration <MailboxName> -EchoGroupMessageBackToSubscribedSender $True`  

<span data-ttu-id="3cd1b-105">Da biste istovremeno omogućili postavku za sve Poštanske sandučiće:</span><span class="sxs-lookup"><span data-stu-id="3cd1b-105">To enable the setting for all mailboxes at once:</span></span>

`Get-Mailbox -ResultSize Unlimited | ForEach {Set-MailboxMessageConfiguration -Identity $_.UserPrincipalName -EchoGroupMessageBackToSubscribedSender $true}` 

<span data-ttu-id="3cd1b-106">**Napomena** Promene ove postavke imaju do trenutka da stupe na snagu.</span><span class="sxs-lookup"><span data-stu-id="3cd1b-106">**Note** Changes to this setting take up to an hour to take effect.</span></span>