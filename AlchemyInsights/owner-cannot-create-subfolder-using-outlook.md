---
title: Vlasnik ne može da kreira podfasciklu pomoću programa Outlook
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5884"
- "3500007"
ms.openlocfilehash: 2116bb837e4378ea29d7882df1d3010b3a4e0b1c
ms.sourcegitcommit: 936330b11fec49f6174eadea6c765bdf9e6ba784
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 06/12/2020
ms.locfileid: "44749143"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a>Vlasnik ne može da kreira podfasciklu pomoću programa Outlook

**Postoji problem sa vlasnicima javnih fascikli koji kreiraju potfascikle pomoću programa Outlook. To pitanje će uskoro biti ispravljeno.**

U međuvremenu, koristite jedno od sledećih rešenja:

1. Korišćenje programa Outlook za MAC za kreiranje potfascikle dok problem utiče samo na Outlook za prozore radne površine (sve verzije)
2. Neka admin napravi potfasciklu koristeći "EXO Shell" ili EAC
3. Promenite DefaultPublicFolderMailbox/EffectivePublicFolderMailbox za korisnika u drugo poštansko sanduče nego poštansko sanduče sadržaja za fasciklu koja uzrokuje problem  
    - *Set-poštansko sanduče User1 DefaultPublicFolderMailbox PubMBX3*
4. Sačekajte sat, ponovo pokrenite Outlook Client