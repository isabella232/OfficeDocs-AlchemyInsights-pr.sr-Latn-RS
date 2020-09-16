---
title: Smernice za zadržavanje u Exchange centru administracije ne funkcionišu
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 1fee2361b2dd6e0989d430a17aebb13bd5948578
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47740524"
---
# <a name="retention-policies-in-exchange-admin-center"></a>Smernice za zadržavanje u Exchange centru administracije

Ako želite da uradite automatizovane provere za postavke navedene ispod, kliknite na dugme nazad <, na vrhu ove stranice, a zatim unesite e-adresu korisnika koji ima problema sa smernicama za zadržavanje.

 **Problem:** Nove kreirane ili ažurirane smernice za zadržavanje u Exchange centru administracije se ne primenjuju na Poštanske sandučiće ili stavke se ne pomeraju u poštansko sanduče arhiva ili izbrisane. 
  
 **Osnovni uzroci:**
  
- To je možda zato što **Pomoćnik kontrolisane fascikle** nije obradio poštansko sanduče korisnika. Pomoćnik kontrolisane fascikle pokušava da obradi svako poštansko sanduče u organizaciji zasnovanoj na oblaku na svakih sedam dana. Ako promenite oznaku za zadržavanje ili primenite različitu polisu za zadržavanje na poštansko sanduče, možete da sačekate dok Kontrolisana fascikla ne obradi poštansko sanduče ili možete da pokrenete program "Start-Managederderderik" koji će obraditi određeno poštansko sanduče. Pokretanje ovog cmdlet funkcije je korisno za testiranje ili rešavanje problema sa postavkama oznake za zadržavanje ili označavanje. Više informacija potražite u odeljku ["Pomoćnik za upravljanje fasciklama](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist)".
    
  - **Rešenje:** Pokrenite sledeću komandu da biste pokrenuli pomoćnika kontrolisane fascikle za određeno poštansko sanduče:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- To se može desiti i ako je **zadržavanje** **omogućeno** na poštanskom sandučetu. Ako je poštansko sanduče postavljeno na čekanje, smernice za zadržavanje na poštanskom sandučetu neće biti obrađene tokom tog vremena. Za više Informatika na stranici zadržavanje pogledajte članak: [čekanje zadržavanja poštanskog sandučeta](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).
    
    **Raspada**
    
  - Potvrdite status postavke zadržavanja na određenom poštanskom sandučetu u [Exo PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - Uradite sledeće komande da biste **onemogućili** čekanje na određeno poštansko sanduče:
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - Sada ponovo vodite pomoćnika kontrolisanog fascikle:
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 **Napomena:** Ako je poštansko sanduče manje od 10 MB, pomoćnik kontrolisane fascikle neće automatski obraditi poštansko sanduče.
 
Više informacija o smernicama za zadržavanje u Exchange centru administracije potražite u članku:
- [Oznake za zadržavanje i smernice za zadržavanje](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [Primenjivanje smernica za zadržavanje na Poštanske sandučiće](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [Dodavanje ili uklanjanje oznaka za zadržavanje](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [Kako da identifikujete tip čekanja postavljeno na poštansko sanduče](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
