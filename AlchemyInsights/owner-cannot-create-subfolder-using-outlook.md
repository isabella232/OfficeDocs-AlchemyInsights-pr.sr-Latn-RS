---
title: Vlasnik ne može da kreira potfasciku pomoću programa Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5884"
- "3500007"
ms.openlocfilehash: b2ab7b60bc521fd28d68333bb963528f7b9e05f2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/15/2021
ms.locfileid: "51836149"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a>Vlasnik ne može da kreira potfasciku pomoću programa Outlook

**Postoji tekući problem sa vlasnicima javnih fascikli koji prave potfascikle pomoću programa Outlook. Problem će uskoro biti rešen.**

U međuvremenu koristite neko od sledećih zaokreta:

1. Korišćenje programa Outlook za MAC za kreiranje potfascikle jer problem utiče samo na Outlook za windows računare (sve verzije)
2. Kreiranje potfascikle pomoću programa EXO Shell ili EAC
3. Promena defaultPublicFolderMailbox/EffectivePublicFolderMailbox korisnika u drugo poštansko sanduče nego poštansko sanduče sadržaja za fasciklu koja uzrokuje problem  
    - *Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*
4. Sačekajte sat vremena, ponovo pokrenite Outlook klijent