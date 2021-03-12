---
title: Nije moguće poslati/primiti e-poštu na/iz sistema Office 365 zbog TLS 1,0 i TLS 1,1 umanjenja
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9005383"
- "9275"
ms.openlocfilehash: 9927112608ae58751e43c1bf0592fbd4a7cf1a0e
ms.sourcegitcommit: be246651064dfeacc866b2f69c0dbe4002a73f1c
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/11/2021
ms.locfileid: "50747118"
---
# <a name="unable-to-sendreceive-email-tofrom-office-365-because-of-the-tls-10-and-tls-11-disablement"></a>Nije moguće poslati/primiti e-poštu na/iz sistema Office 365 zbog TLS 1,0 i TLS 1,1 umanjenja

Kao što je potvrđeno MC229914 centar za poruke, TLS 1,0 i TLS 1,1 ukidanje alatki dsync su započeli primenu za Exchange online protok krajnjih tačaka. Uskoro Office 365 više neće prihvatiti TLS 1,0 i TLS 1,1 veze e-pošte iz spoljnih izvora. Takođe, Exchange online nikada neće koristiti TLS 1,0 ili 1,1 za slanje odlazne e-pošte. Ako se suočavate sa problemima zbog toga što je TLS 1,0 ili 1,1 umanjenje, možda ćete iskusiti jednu od sledećih grešaka –

- Pošiljalac pristupa-' 421 4.4.2 veza je opala zbog protivprotivterorizma '.
- Greška u prikazivaču čekanja lokalnog servera koji šalje e-poštu policajcu 365-' 421 4.4.2 veza je opala zbog dodatka "aktterorizam"
- Greška u slanju [evidencije protokola protokola](https://docs.microsoft.com/exchange/mail-flow/connectors/protocol-logging) slanja konektora na serveru koji šalje e-poštu na Office 365-TLS pregovaranje nije uspelo sa Akakterorističkom Error
- Greška u dnevniku konektora za slanje ili prijem protokola veze-' 451 5.7.3 mora prvo da izda prvu komandu '

Ako nailazite na neku od gorenavedenih grešaka, proverite da li server koji šalje ili prima e-poštu ima TLS 1,2 omogućena pomoću sledećih registarskih ključeva

[HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1,2] [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2 \ klijent] **"Onemogućavanje" "= DWORD: 00000000" omogućeno "= DWORD: 00000001** [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2 \ server] **" Onemogući "onemogućavanje" = DWORD: 00000000 "omogućeno" = DWORD: 00000001**

Ako napravite bilo kakvu promenu u gorenavedenim registarskim 1,2 kljuиevima, pokrenite server da bi promene stupile na snagu. Uverite se i da imate instalirane najnovije Windows i Exchange ispravke.

Za više informacija pogledajte članak:

- [Vodič za Exchange Server TLS, deo 1: priprema za TLS 1,2-Microsoft Tech Community](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-1-getting-ready-for-tls-1-2/ba-p/607649)
- [Vodič za Exchange Server TLS deo 2: omogućavanje TLS 1,2 i identifikovanje klijenata koji ne koriste IT – Microsoft Tech Community](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-2-enabling-tls-1-2-and/ba-p/607761)
- [Razumevanje scenarija e-pošte ako nije moguće složiti se sa TLS verzijama pomoću Exchange online-Microsoft Tech zajednice](https://techcommunity.microsoft.com/t5/exchange-team-blog/understanding-email-scenarios-if-tls-versions-cannot-be-agreed/ba-p/2065089)
