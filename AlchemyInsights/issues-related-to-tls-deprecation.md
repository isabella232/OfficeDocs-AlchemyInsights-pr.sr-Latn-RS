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
# <a name="unable-to-sendreceive-email-tofrom-office-365-because-of-the-tls-10-and-tls-11-disablement"></a><span data-ttu-id="54764-102">Nije moguće poslati/primiti e-poštu na/iz sistema Office 365 zbog TLS 1,0 i TLS 1,1 umanjenja</span><span class="sxs-lookup"><span data-stu-id="54764-102">Unable to send/receive email to/from Office 365 because of the TLS 1.0 and TLS 1.1 disablement</span></span>

<span data-ttu-id="54764-103">Kao što je potvrđeno MC229914 centar za poruke, TLS 1,0 i TLS 1,1 ukidanje alatki dsync su započeli primenu za Exchange online protok krajnjih tačaka.</span><span class="sxs-lookup"><span data-stu-id="54764-103">As confirmed by the message center post MC229914, TLS 1.0 and TLS 1.1 deprecation started enforcing for Exchange Online mail flow endpoints.</span></span> <span data-ttu-id="54764-104">Uskoro Office 365 više neće prihvatiti TLS 1,0 i TLS 1,1 veze e-pošte iz spoljnih izvora.</span><span class="sxs-lookup"><span data-stu-id="54764-104">Soon Office 365 will no longer accept TLS 1.0 and TLS 1.1 email connections from external sources.</span></span> <span data-ttu-id="54764-105">Takođe, Exchange online nikada neće koristiti TLS 1,0 ili 1,1 za slanje odlazne e-pošte.</span><span class="sxs-lookup"><span data-stu-id="54764-105">Also, Exchange Online will never use TLS 1.0 or 1.1 to send outbound email.</span></span> <span data-ttu-id="54764-106">Ako se suočavate sa problemima zbog toga što je TLS 1,0 ili 1,1 umanjenje, možda ćete iskusiti jednu od sledećih grešaka –</span><span class="sxs-lookup"><span data-stu-id="54764-106">If you are facing issues because of TLS 1.0 or 1.1 disablement, you might experience one of the following errors-</span></span>

- <span data-ttu-id="54764-107">Pošiljalac pristupa-' 421 4.4.2 veza je opala zbog protivprotivterorizma '.</span><span class="sxs-lookup"><span data-stu-id="54764-107">Sender is getting NDR bounce back - '421 4.4.2 Connection dropped due to SocketError'</span></span>
- <span data-ttu-id="54764-108">Greška u prikazivaču čekanja lokalnog servera koji šalje e-poštu policajcu 365-' 421 4.4.2 veza je opala zbog dodatka "aktterorizam"</span><span class="sxs-lookup"><span data-stu-id="54764-108">Error in the Queue Viewer of On-Premises server that is sending email to Officer 365- '421 4.4.2 Connection dropped due to SocketError'</span></span>
- <span data-ttu-id="54764-109">Greška u slanju [evidencije protokola protokola](https://docs.microsoft.com/exchange/mail-flow/connectors/protocol-logging) slanja konektora na serveru koji šalje e-poštu na Office 365-TLS pregovaranje nije uspelo sa Akakterorističkom Error</span><span class="sxs-lookup"><span data-stu-id="54764-109">Error in Send connector [Protocol log](https://docs.microsoft.com/exchange/mail-flow/connectors/protocol-logging) on the server sending email to Office 365- TLS negotiation failed with error SocketError</span></span>
- <span data-ttu-id="54764-110">Greška u dnevniku konektora za slanje ili prijem protokola veze-' 451 5.7.3 mora prvo da izda prvu komandu '</span><span class="sxs-lookup"><span data-stu-id="54764-110">Error in Send or receive connector protocol log - '451 5.7.3 Must issue a STARTTLS command first'</span></span>

<span data-ttu-id="54764-111">Ako nailazite na neku od gorenavedenih grešaka, proverite da li server koji šalje ili prima e-poštu ima TLS 1,2 omogućena pomoću sledećih registarskih ključeva</span><span class="sxs-lookup"><span data-stu-id="54764-111">If you experience any of the above errors, please make sure the server that is sending or receiving email has TLS 1.2 enabled by checking the following registry keys-</span></span>

<span data-ttu-id="54764-112">[HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1,2] [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2 \ klijent] **"Onemogućavanje" "= DWORD: 00000000" omogućeno "= DWORD: 00000001** [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2 \ server] **" Onemogući "onemogućavanje" = DWORD: 00000000 "omogućeno" = DWORD: 00000001**</span><span class="sxs-lookup"><span data-stu-id="54764-112">[HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2] [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Client] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001** [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Server] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001**</span></span>

<span data-ttu-id="54764-113">Ako napravite bilo kakvu promenu u gorenavedenim registarskim 1,2 kljuиevima, pokrenite server da bi promene stupile na snagu.</span><span class="sxs-lookup"><span data-stu-id="54764-113">If you make any change in the above registry keys to enable TLS 1.2, restart the server for the changes to take effect.</span></span> <span data-ttu-id="54764-114">Uverite se i da imate instalirane najnovije Windows i Exchange ispravke.</span><span class="sxs-lookup"><span data-stu-id="54764-114">Also make sure you have the latest Windows and Exchange updates installed.</span></span>

<span data-ttu-id="54764-115">Za više informacija pogledajte članak:</span><span class="sxs-lookup"><span data-stu-id="54764-115">For more information, see:</span></span>

- [<span data-ttu-id="54764-116">Vodič za Exchange Server TLS, deo 1: priprema za TLS 1,2-Microsoft Tech Community</span><span class="sxs-lookup"><span data-stu-id="54764-116">Exchange Server TLS guidance, part 1: Getting Ready for TLS 1.2 - Microsoft Tech Community</span></span>](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-1-getting-ready-for-tls-1-2/ba-p/607649)
- [<span data-ttu-id="54764-117">Vodič za Exchange Server TLS deo 2: omogućavanje TLS 1,2 i identifikovanje klijenata koji ne koriste IT – Microsoft Tech Community</span><span class="sxs-lookup"><span data-stu-id="54764-117">Exchange Server TLS guidance Part 2: Enabling TLS 1.2 and Identifying Clients Not Using It - Microsoft Tech Community</span></span>](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-2-enabling-tls-1-2-and/ba-p/607761)
- [<span data-ttu-id="54764-118">Razumevanje scenarija e-pošte ako nije moguće složiti se sa TLS verzijama pomoću Exchange online-Microsoft Tech zajednice</span><span class="sxs-lookup"><span data-stu-id="54764-118">Understanding email scenarios if TLS versions cannot be agreed on with Exchange Online - Microsoft Tech Community</span></span>](https://techcommunity.microsoft.com/t5/exchange-team-blog/understanding-email-scenarios-if-tls-versions-cannot-be-agreed/ba-p/2065089)
