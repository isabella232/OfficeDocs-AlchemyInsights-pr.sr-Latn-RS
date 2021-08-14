---
title: Vlasnik ne može da napravi potfasciku korišćenjem Outlook
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
ms.openlocfilehash: 60190727e75c120ad3915da8b563b7f6b1a3238b46bb6e14cbf956365e1a84e0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "54063138"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a>Vlasnik ne može da napravi potfasciku korišćenjem Outlook

**Postoji tekući problem sa vlasnicima javnih fascikli koji prave potfascikle pomoću Outlook. Problem će uskoro biti rešen.**

U međuvremenu koristite neko od sledećih zaokreta:

1. Koristite Outlook za MAC da biste kreirali potfasciklu jer problem utiče samo na Outlook radne površine za stone računare (sve verzije)
2. Kreiranje potfascikle pomoću programa EXO Shell ili EAC
3. Promena defaultPublicFolderMailbox/EffectivePublicFolderMailbox korisnika u drugo poštansko sanduče nego poštansko sanduče sadržaja za fasciklu koja uzrokuje problem  
    - *Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*
4. Sačekajte sat vremena, ponovo pokrenite Outlook klijent