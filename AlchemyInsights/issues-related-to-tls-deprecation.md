---
title: Nije moguće slanje/prijem e-pošte za/od Office 365 zbog onemogućavanja TLS 1.0 i TLS 1.1
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
ms.openlocfilehash: 508e48fd0e46557de075f4752da017ab8cc326923a965350140e598f7f7cf557
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "54054920"
---
# <a name="unable-to-sendreceive-email-tofrom-office-365-because-of-the-tls-10-and-tls-11-disablement"></a>Nije moguće slanje/prijem e-pošte za/od Office 365 zbog onemogućavanja TLS 1.0 i TLS 1.1

Kao što je potvrdila objava centra za poruke MC229914, ukidanje TLS 1.0 i TLS 1.1 započelo je pojačavanje za krajnje tačke protoka pošte Exchange Online pošte. Uskoro Office 365 više neće prihvatati TLS 1.0 i TLS 1.1 veze e-pošte iz spoljnih izvora. Takođe, Exchange Online nikada neće koristiti TLS 1.0 ili 1.1 za slanje odlazne e-pošte. Ako imate problema zbog onemogućavanja TLS 1.0 ili 1.1, može da se pojavi jedna od sledećih grešaka:

- Sender is getting NDR bounce back - '421 4.4.2 Connection dropped due to SocketError'
- Greška u prikazivaču na čekanju na unutrašnjem serveru koja šalje e-poštu službenici 365- "421 4.4.2 Veza je zakačena zbog greške SocketError"
- Greška u evidenciji [protokola](https://docs.microsoft.com/exchange/mail-flow/connectors/protocol-logging) slanja konektora na serveru koji šalje e-poštu na Office 365- TLS pregovaranje nije uspelo uz grešku SocketError
- Greška u evidenciji protokola slanja ili prijema konektora - "451 5.7.3 Mora prvo da izda KOMANDU STARTTLS"

Ako naiđete na neku od gorenavedenih grešaka, proverite da li je server koji šalje ili prima e-poštu omogućen TLS 1.2 tako što ćete proveriti sledeće ključeve registratora-

[HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1,2] [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Client] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001** [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Server] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001**

Ako promenite navedene ključeve registratora da biste omogućili TLS 1.2, ponovo pokrenite server da bi promene stupile na snagu. Takođe se uverite da imate instalirane najnovije Windows i Exchange ispravki.

Za više informacija pogledajte:

- [Exchange server TLS uputstvo, 1. deo: Priprema za TLS 1.2 – Microsoft Tech zajednica](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-1-getting-ready-for-tls-1-2/ba-p/607649)
- [Exchange server TLS guidance Part 2: Omogućavanje TLS 1.2 i identifikovanje klijenata koji ga ne koriste – Microsoft Tech Community](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-2-enabling-tls-1-2-and/ba-p/607761)
- [Razumevanje scenarija e-pošte ako nije moguće pristati na TLS verzije sa Exchange Online – Microsoft Tech Community](https://techcommunity.microsoft.com/t5/exchange-team-blog/understanding-email-scenarios-if-tls-versions-cannot-be-agreed/ba-p/2065089)
