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
# <a name="sender-does-not-receive-email-sent-to-microsoft-365-group"></a>Pošiljalac ne prima e-poštu koja se šalje u Microsoft 365 grupi

Pošiljalac e-365 poruke podrazumevano ne prima kopiju poruke u prijemnom poštanskom sandučetu, čak i ako je pošiljalac član grupe.

Koristite ovu komandu EXO PowerShell da biste omogućili pošiljaocu da primi kopiju svake e-poruke koju pošalju u Microsoft 365 grupu:  

`Set-MailboxMessageConfiguration <MailboxName> -EchoGroupMessageBackToSubscribedSender $True`  

Da biste istovremeno omogućili postavku za sve Poštanske sandučiće:

`Get-Mailbox -ResultSize Unlimited | ForEach {Set-MailboxMessageConfiguration -Identity $_.UserPrincipalName -EchoGroupMessageBackToSubscribedSender $true}` 

**Napomena** Promene ove postavke imaju do trenutka da stupe na snagu.