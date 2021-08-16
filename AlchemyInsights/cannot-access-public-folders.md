---
title: Nije moguće pristupiti javnim fasciklama
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: f129da8731877aa00fd9b1dcf20905d353a4895303390ce7ff5642a8ff3ccbc2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "53996644"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Outlook povezivanje sa javnim fasciklama

Ako pristup javnoj fascikli ne funkcioniše za neke korisnike, pokušajte sledeće:

Povezivanje na EXO PowerShell i konfigurišite Parametar DefaultPublicFolderMailbox na korisničkom nalogu problema tako da se podudara sa parametarom na radnom korisničkom nalogu.

Primer:

Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox

Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command>

Sačekajte najmanje jedan čas da bi promena stupila na snagu.

Ako problem ostane, pratite ovu proceduru [da](https://aka.ms/pfcte) biste rešili probleme sa pristupom javnim fasciklama pomoću Outlook.
 
**Da biste kontrolisali koji korisnici mogu da pristupe javnim fasciklama Outlook:**

1.  Koristite Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true ili $false  
      
    $true: Omogućite korisnicima da pristupe javnim fasciklama u Outlook  
      
    $false: Sprečite korisnički pristup javnim fasciklama u Outlook. Ovo je podrazumevana vrednost.  
        
2.  Set-OrganizationConfig -PublicFolderShowClientControl $true   
      
**Napomišite** Ova procedura može da kontroliše veze samo sa Outlook na radnoj površini Windows klijentima. Korisnik može da nastavi da pristupa javnim fasciklama koristeći program OWA Outlook za Mac.
 
Više informacija potražite u [članku Najavljivanje podrške za kontrolisane](https://aka.ms/controlpf)veze sa javnim fasciklama u programu Outlook.