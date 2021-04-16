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
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a>Greška pri slanju e-pošte: Host klijenta je blokiran koristeći Spamhaus

IP adresa sa koje je poslata poruka nalazi se na listi blokiranih objekata koja je u vlasništvu [sajta Spamhaus.](https://go.microsoft.com/fwlink/p/?linkid=123245) Razlozi zbog kojih bi vas Spamhaus blokirao uključuju ugrožene naloge, ugrožene računare koji dele javnu IP adresu i smernice dobavljača internet usluga (ISP). Moguća ispravka su:
  
- Za blokirane dolazne poruke u kojima kontrolišete izvorni server e-pošte, morate da utvrdite uzrok i uklonite blokiranje sa veb sajta Spamhaus.

- Za blokirane dolazne poruke u kojima izvorna IP adresa pripada nekom drugom, vlasnik adrese mora da ukloni blokiranje sa veb sajta Spamhaus. Ako je IP adresa na listi blokiranja smernica (PBL), vlasnik može da dodeli različitu statičnu IP adresu ili ukloni adresu sa PBL liste.

- Za blokirane odlazne poruke sa vašeg domena povezanog sa korporacijom Microsoft, ovu grešku možete dobiti ako se poruke usmere putem usluge nezavisnog dobavljača. Možete da koristite alatku za pronalaženje KO JE KO da biste pronašli vlasnika blokirane IP adrese.
