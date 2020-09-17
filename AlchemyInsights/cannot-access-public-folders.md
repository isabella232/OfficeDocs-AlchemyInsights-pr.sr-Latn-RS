---
title: Nije moguće pristupiti javnim fasciklama
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: 272918b38f6019cb2bdcaa4013baebaa5f04fe85
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/15/2020
ms.locfileid: "47812561"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Outlook ne može da se poveže sa javnim fasciklama

Ako pristup javnoj fascikli ne radi za neke korisnike, Isprobajte sledeće:

Povežite se sa EXO PowerShell i konfigurišite parametar Defaultpublicfolfoldersanduče na problem korisničkog naloga da bi se podudarao sa parametrima na radnom korisničkom nalogu.

Primer

Rešenje "Uzmi-poštansko sanduče" | FT Defaultpublicfolfolderpoštansko sanduče, efikasno iskorišćenost poštanskog sandučeta

Komplet-problem sa poštanskim sandučetom-Defaultpublicfoldersanduče \<value from previous command>

Sačekajte najmanje jedan sat da bi promena stupila na snagu.

Ako problem ostane, pratite [ovu proceduru](https://aka.ms/pfcte) da biste rešili probleme sa pristupom javnoj fascikli pomoću programa Outlook.
 
**Da biste kontrolisali koji korisnici mogu da pristupe javnim fasciklama pomoću programa Outlook**:

1.  Koristite setu- <mailboxname> Kaskadepoštansko sanduče-publicfolderclientaccess $TRUE ili $FALSE  
      
    $true: Omogućavanje korisnicima da pristupaju javnim fasciklama u programu Outlook  
      
    $false: sprečite korisnički pristup javnim fasciklama u programu Outlook. Ovo je podrazumevana vrednost.  
        
2.  Scenokonfiguracija – Publicfoldershow$TRUE   
      
**Napomena** Ova procedura može da kontroliše veze samo sa Outlook klijentima za računare za Windows. Korisnik može da nastavi pristup javnim fasciklama pomoću aplikacije OWA ili Outlook za Mac.
 
Više informacija potražite u članku [Najavljujemo podršku za kontrolisane veze ka javnim fasciklama u programu Outlook](https://aka.ms/controlpf).