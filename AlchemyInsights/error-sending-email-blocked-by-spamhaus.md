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
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a>Greška prilikom slanja e-pošte: klijent host je blokiran koristeći spamhaus

IP adresa koja je poslata je na listu blokova u vlasništvu [spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245). Razlozi za blokiranje spamhaus-a obuhvataju kompromitovane naloge, ugrožene mašine koje dele javnu IP adresu i smernice dobavljača Internet usluga (ISP). Moguće ispravke su:
  
- Za blokirane dolazne poruke u kojima kontrolišete izvorni server e-pošte, morate da utvrdite uzrok i uklonite blok sa Veb lokacije spamhaus.

- Za blokirane dolazne poruke gde izvorna IP adresa pripada nekom drugom, vlasnik adrese mora da ukloni blok sa Veb lokacije spamhaus. Ako se IP adresa nalazi na listi blokiranih smernica (PBL), vlasnik može da dodeli različitu IP adresu ili da ukloni adresu iz PBL.

- Za blokirane odlazne poruke iz domena povezane sa korporacijom Microsoft, možete da primite ovu grešku ako se poruke usmeravaju preko usluge nezavisnog proizvođača. Možete da koristite kois alatku za pronalaženje da biste pronašli blokirani vlasnik IP adrese.
