---
title: Greška prilikom slanja e-pošte koja je blokirala SpamHaus
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: a0c2f4be0b2d8ba6fd3dadbdf306e6ce623ad380
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/15/2020
ms.locfileid: "47783817"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a><span data-ttu-id="6baf0-102">Greška prilikom slanja e-pošte: klijent host je blokiran koristeći spamhaus</span><span class="sxs-lookup"><span data-stu-id="6baf0-102">Error sending email: Client host blocked using Spamhaus</span></span>

<span data-ttu-id="6baf0-103">IP adresa koja je poslata je na listu blokova u vlasništvu [spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span><span class="sxs-lookup"><span data-stu-id="6baf0-103">The IP address that sent the message is on a block list owned by [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span></span> <span data-ttu-id="6baf0-104">Razlozi za blokiranje spamhaus-a obuhvataju kompromitovane naloge, ugrožene mašine koje dele javnu IP adresu i smernice dobavljača Internet usluga (ISP).</span><span class="sxs-lookup"><span data-stu-id="6baf0-104">Reasons for being blocked by Spamhaus include compromised accounts, compromised machines sharing a public IP address, and Internet Service Provider (ISP) policies.</span></span> <span data-ttu-id="6baf0-105">Moguće ispravke su:</span><span class="sxs-lookup"><span data-stu-id="6baf0-105">Possible fixes are:</span></span>
  
- <span data-ttu-id="6baf0-106">Za blokirane dolazne poruke u kojima kontrolišete izvorni server e-pošte, morate da utvrdite uzrok i uklonite blok sa Veb lokacije spamhaus.</span><span class="sxs-lookup"><span data-stu-id="6baf0-106">For blocked inbound messages where you control the source email server, you need to determine the cause and remove the block from the Spamhaus website.</span></span>

- <span data-ttu-id="6baf0-107">Za blokirane dolazne poruke gde izvorna IP adresa pripada nekom drugom, vlasnik adrese mora da ukloni blok sa Veb lokacije spamhaus.</span><span class="sxs-lookup"><span data-stu-id="6baf0-107">For blocked inbound messages where the source IP address belongs to someone else, the address owner needs to remove the block from the Spamhaus website.</span></span> <span data-ttu-id="6baf0-108">Ako se IP adresa nalazi na listi blokiranih smernica (PBL), vlasnik može da dodeli različitu IP adresu ili da ukloni adresu iz PBL.</span><span class="sxs-lookup"><span data-stu-id="6baf0-108">If the IP address is on the Policy Block List (PBL), the owner can assign a different static IP address or remove the address from the PBL.</span></span>

- <span data-ttu-id="6baf0-109">Za blokirane odlazne poruke iz domena povezane sa korporacijom Microsoft, možete da primite ovu grešku ako se poruke usmeravaju preko usluge nezavisnog proizvođača.</span><span class="sxs-lookup"><span data-stu-id="6baf0-109">For blocked outbound messages from your domain connected to Microsoft, you can receive this error if the messages are routed through a 3rd party service.</span></span> <span data-ttu-id="6baf0-110">Možete da koristite kois alatku za pronalaženje da biste pronašli blokirani vlasnik IP adrese.</span><span class="sxs-lookup"><span data-stu-id="6baf0-110">You can use a WHOIS lookup tool to find the blocked IP address owner.</span></span>
