---
title: Greška pri slanju e-pošte koja je blokirala SpamHaus
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "255"
- "3100003"
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 8b5ac1df0b6a07a475345235a8b4b555d6881147
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813738"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a><span data-ttu-id="de938-102">Greška pri slanju e-pošte: Host klijenta je blokiran koristeći Spamhaus</span><span class="sxs-lookup"><span data-stu-id="de938-102">Error sending email: Client host blocked using Spamhaus</span></span>

<span data-ttu-id="de938-103">IP adresa sa koje je poslata poruka nalazi se na listi blokiranih objekata koja je u vlasništvu [sajta Spamhaus.](https://go.microsoft.com/fwlink/p/?linkid=123245)</span><span class="sxs-lookup"><span data-stu-id="de938-103">The IP address that sent the message is on a block list owned by [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span></span> <span data-ttu-id="de938-104">Razlozi zbog kojih bi vas Spamhaus blokirao uključuju ugrožene naloge, ugrožene računare koji dele javnu IP adresu i smernice dobavljača internet usluga (ISP).</span><span class="sxs-lookup"><span data-stu-id="de938-104">Reasons for being blocked by Spamhaus include compromised accounts, compromised machines sharing a public IP address, and Internet Service Provider (ISP) policies.</span></span> <span data-ttu-id="de938-105">Moguća ispravka su:</span><span class="sxs-lookup"><span data-stu-id="de938-105">Possible fixes are:</span></span>
  
- <span data-ttu-id="de938-106">Za blokirane dolazne poruke u kojima kontrolišete izvorni server e-pošte, morate da utvrdite uzrok i uklonite blokiranje sa veb sajta Spamhaus.</span><span class="sxs-lookup"><span data-stu-id="de938-106">For blocked inbound messages where you control the source email server, you need to determine the cause and remove the block from the Spamhaus website.</span></span>

- <span data-ttu-id="de938-107">Za blokirane dolazne poruke u kojima izvorna IP adresa pripada nekom drugom, vlasnik adrese mora da ukloni blokiranje sa veb sajta Spamhaus.</span><span class="sxs-lookup"><span data-stu-id="de938-107">For blocked inbound messages where the source IP address belongs to someone else, the address owner needs to remove the block from the Spamhaus website.</span></span> <span data-ttu-id="de938-108">Ako je IP adresa na listi blokiranja smernica (PBL), vlasnik može da dodeli različitu statičnu IP adresu ili ukloni adresu sa PBL liste.</span><span class="sxs-lookup"><span data-stu-id="de938-108">If the IP address is on the Policy Block List (PBL), the owner can assign a different static IP address or remove the address from the PBL.</span></span>

- <span data-ttu-id="de938-109">Za blokirane odlazne poruke sa vašeg domena povezanog sa korporacijom Microsoft, ovu grešku možete dobiti ako se poruke usmere putem usluge nezavisnog dobavljača.</span><span class="sxs-lookup"><span data-stu-id="de938-109">For blocked outbound messages from your domain connected to Microsoft, you can receive this error if the messages are routed through a 3rd party service.</span></span> <span data-ttu-id="de938-110">Možete da koristite alatku za pronalaženje KO JE KO da biste pronašli vlasnika blokirane IP adrese.</span><span class="sxs-lookup"><span data-stu-id="de938-110">You can use a WHOIS lookup tool to find the blocked IP address owner.</span></span>
