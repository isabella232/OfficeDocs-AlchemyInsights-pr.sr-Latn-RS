---
title: Pošalji kao Microsoft 365 grupa
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/19/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
ms.openlocfilehash: cfb4bd5ce59eeccdd0812d013b8a444aebeb1d4c
ms.sourcegitcommit: 9818d3c8e6b10f23244e51286e2463caf48fffd5
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/21/2020
ms.locfileid: "46872120"
---
# <a name="send-as-microsoft-365-group"></a>Pošalji kao Microsoft 365 grupa

Možete dodeliti dozvole "Pošalji kao" da biste omogućili određenim korisnicima da šalju poruke kao grupu Microsoft 365:  

1. Povezivanje sa uslugom Exchange online PowerShell.  

2. Uradite sledeće:  

    Add-RecipientPermission `<GroupName>` -Poverenit `<MailboxName>` sendas

Više informacija potražite u članku [Omogućavanje članovima za slanje ili slanje u ime grupe](https://docs.microsoft.com/microsoft-365/admin/create-groups/allow-members-to-send-as-or-send-on-behalf-of-group?view=o365-worldwide).