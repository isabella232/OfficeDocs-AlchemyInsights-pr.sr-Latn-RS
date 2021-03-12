---
title: 1:1 snimanje poziva
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/18/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002530"
- "7648"
ms.openlocfilehash: af09e8805409446a42a62c82aa577ad27f09a17a
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/11/2021
ms.locfileid: "50733863"
---
# <a name="11-call-recording"></a>1:1 snimanje poziva

Administratori sada treba da preduzmu korake da bi nastavili da omogućavaju korisnicima da snimaju 1:1 pozive.
 
Počevši od 2012, 2021, počinjemo da sprovodimo nove timove koji pozivaju *na opciju* 

Trenutno 1:1 mogućnosti snimanja poziva kontroliše se opcija *Allowda Drekording* u smernicama timova za sastanak. Ako je korisnicima dozvoljeno da snimaju sastanke tima, takođe mogu da snime 1:1 pozive.

Ako želite da blokirate sve korisnike da snimaju 1:1 pozive, ne morate da preduzimate nikakve radnje. Opcija *Allowza Drecordingforpozivi* će podrazumevano biti $FALSE.

Ova promena je dokumentovana u sledećem objavljenoj centru za poruke: [(ažurirano) 1:1 Call smernice za zapisivanje smernica](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796) za postavljanje opcije "timovi za pozivanje" morate da koristite [PowerShell](https://docs.microsoft.com/microsoftteams/teams-powershell-install).

**Da biste omogućili snimanje poziva u 1:1 pozivima:** Set-CsTeamsCallingPolicy-opšti identitet $TRUE

**Da biste onemogućili snimanje poziva u 1:1 pozivima:** $FALSE Set-CsTeamsCallingPolicy

