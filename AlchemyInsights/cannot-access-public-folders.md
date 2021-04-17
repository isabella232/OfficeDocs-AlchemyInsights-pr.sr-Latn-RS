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
ms.openlocfilehash: af5bd57512ee917d6e22d3838d55a2a1d62750d4
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819526"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Outlook ne može da se poveže sa javnim fasciklama

Ako pristup javnoj fascikli ne funkcioniše za neke korisnike, pokušajte sledeće:

Povežite se sa EXO PowerShell i konfigurišite DefaultPublicFolderMailbox parametar na problemnom korisničkom nalogu da bi se podudarao sa parametarom na radnom korisničkom nalogu.

Primer:

Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox

Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command>

Sačekajte najmanje jedan čas da bi promena stupila na snagu.

Ako problem ostane, pratite ovu proceduru da biste rešili [probleme](https://aka.ms/pfcte) sa pristupom javnoj fascikli pomoću programa Outlook.
 
**Da biste kontrolisali koji korisnici mogu da pristupe javnim fasciklama pomoću programa Outlook:**

1.  Koristite Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true ili $false  
      
    $true: Dozvoljavanje korisnicima da pristupe javnim fasciklama u programu Outlook  
      
    $false: Sprečite korisnički pristup javnim fasciklama u programu Outlook. Ovo je podrazumevana vrednost.  
        
2.  Set-OrganizationConfig -PublicFolderShowClientControl $true   
      
**Napomišite** Ova procedura može da kontroliše veze samo sa Outlook klijentima za računare za Windows. Korisnik može da nastavi da pristupa javnim fasciklama koristeći program OWA ili Outlook za Mac.
 
Više informacija potražite u [članku Najavljivanje podrške za kontrolisane veze sa javnim fasciklama u programu Outlook.](https://aka.ms/controlpf)