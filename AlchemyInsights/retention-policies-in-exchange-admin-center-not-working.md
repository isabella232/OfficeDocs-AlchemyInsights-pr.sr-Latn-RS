---
title: Smernice za zadržavanje u sistemu Exchange admin Center ne rade
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 4d3ca121c8d22a0900f136f7f2a754dfb5b435f5
ms.sourcegitcommit: ffbed67c0a16ec423fa1d79b71e48ea4e2d320e1
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 07/29/2020
ms.locfileid: "46522821"
---
# <a name="retention-policies-in-exchange-admin-center"></a>Smernice za zadržavanje u programu Exchange admin Center

Ako želite da pokrećemo automatske provere za gore pomenute postavke, kliknite na dugme "nazad" <--na vrhu ove stranice, a zatim unesite e-adresu korisnika koji ima problema sa smernicama za zadržavanje.

 **Problem:** Nove ili ažurirane smernice za zadržavanje u Exchange admin Center ne primenjuju se na Poštanske sandučiće ili stavke nisu premeštene u poštansko sanduče arhive ili su izbrisane. 
  
 **Osnovni uzroci:**
  
- Ovo je možda zbog toga što **Pomoćnik kontrolisane fascikle** nije obradio korisnikovo poštansko sanduče. Pomoćnik kontrolisane fascikle pokušava da obradi svako poštansko sanduče u organizaciji zasnovanom na informatičkom oblaku jednom u sedam dana. Ako promenite oznaku za zadržavanje ili primenite drugačije smernice za zadržavanje u poštansko sanduče, možete sačekati da Kontrolisana fascikla pomogne u obradi poštanskog sandučeta, ili možete da pokrenete Start-ManagedFolderAssistant cmdda biste pokrenuli pomoćnik za kontrolisane fascikle da biste obradili određeno poštansko sanduče. Pokretanje ove cmdmo komande je korisno za testiranje ili rešavanje problema sa postavkama za zadržavanje ili za zadržavanje oznaka zadržavanja. Za više informacija posjetite [pokrenite pomoćnika za Upravljnju fasciklu](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).
    
  - **Rešenje:** Pokrenite sledeću komandu da biste pokrenuli pomoćnik za kontrolisane fascikle za određeno poštansko sanduče:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- Do ovoga može doći i ako je u poštanskom sandučetu **omogućen** **retencionent** . Ako je poštansko sanduče postavljeno na Retencioniku, smernice za zadržavanje u poštanskom sandučetu neće biti obrađene u tom trenutku. Za dodatne informacije o postavci Retentionzadrške pogledajte: [zadržavanje poštanskog sandučeta](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).
    
    **Rešenje:**
    
  - Proverite status postavke Retentiondržanja na određenom poštanskom sandučetu u [Exo PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - Pokrenite sledeću komandu da biste **onemogućili** retentioniste na određenom poštanskom sandučetu:
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - Sada ponovo pokrenite pomoćnika za upravljane fascikle:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 **Napomena:** Ako je poštansko sanduče manje od 10 MB, pomoćnik za Upravljnu fasciklu neće automatski obraditi poštansko sanduče.
 
Više informacija o smernicama za zadržavanje u Exchange admin Center potražite u članku:
- [Zadržavanjem oznaka i smernica zadržavanja](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [Primenjivanje smernica za zadržavanje u Poštanske sandučiće](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [Dodavanje ili uklanjanje oznaka za zadržavanje](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [Identifikovanje tipa zadrška koji se postavlja u poštansko sanduče](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
