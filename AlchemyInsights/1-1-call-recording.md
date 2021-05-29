---
title: 1:1 snimak poziva
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
ms.openlocfilehash: 8cdadf34a059856338d7f40528446b70373465e4
ms.sourcegitcommit: d2108b13acc44e26b65f9a2739cbce9bf98959a5
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 05/28/2021
ms.locfileid: "52702104"
---
# <a name="11-call-recording"></a>1:1 snimak poziva

Ako je **dugme Započni** snimanje zasivo u pozivu 1:1, morate da promenite postavke smernica za korisnika na koje ovo utiče. Da biste proverili postavku smernica, pokrenite dijagnostiku za na uticajnog korisnika tako što će ukucati **Dijag: Teams 1:1 Snimanje** poziva iznad.     

Počejući od 31. maja 2021. počećemo da nalažemo nove smernice za Teams smernica za pozivanje *AllowCloudRecordingForCalls.* Pre ove promene, snimanje poziva 1:1 kontroliše *AllowCloudRecording* Teams za sastanke. Ova promena je dokumentovana u objavi centra za poruke: [(Ažurirano) 1:1](https://portal.microsoft.com/Adminportal/Home?ref=MessageCenter/:/messages/MC238796)Uvod u smernice za snimanje poziva .  

*AllowCloudRecordingForCalls*   opcija smernica pozivanja je **podrazumevano $False** podešena na vrednost . Ako biste radije da blokirate svim korisnicima snimanje 1:1 poziva, ne morate ništa da preduzmete.  

Da biste omogućili snimanje poziva za sve korisnike u 1:1 [pozivima, koristite Teams PowerShell](/microsoftteams/teams-powershell-install) da pokrenete sledeću cmdlet Teams: 

**Set-CsTeamsCallingPolicy -Identity Global -AllowCloudRecordingForCalls $True** 

Druga mogućnost je da kreirate nove smernice i postavite **-AllowCloudRecordingForCalls** **da $true** te smernice dodelili korisnicima. 

Više informacija potražite u 1:1 Kontrole smernica za snimanje poziva [su (Gotovo!) Ovde](https://techcommunity.microsoft.com/t5/microsoft-teams-support/1-1-call-recording-policy-controls-are-almost-here/ba-p/2217668).
