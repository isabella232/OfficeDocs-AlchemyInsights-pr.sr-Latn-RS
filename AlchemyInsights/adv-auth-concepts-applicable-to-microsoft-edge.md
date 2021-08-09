---
title: Napredni koncepti potvrde identiteta koji se primenjuju na Microsoft Edge
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9003931"
- "6986"
- "8329"
- "9004625"
ms.openlocfilehash: 8ddec37260ec4e3bcc390dcc8adb7397368de19555ee31be458be033d3886386
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "53934379"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a>Napredni koncepti potvrde identiteta koji se primenjuju na Microsoft Edge

Slede napredni koncepti potvrde identiteta koji su primenljivi na Microsoft Edge:

**Proaktivna potvrda identiteta**

Kada omogućite [smernice ProactiveAuthEnabled,](https://go.microsoft.com/fwlink/?linkid=2134621) Microsoft Edge će pokušati da proaktivno potvrdi identitet prijavljenih korisnika putem Microsoft usluge. U redovnim intervalima koristiće uslugu na mreži da bi proverila ažuriranu manifest koja sadrži konfiguraciju koja upravlja Proaktivnom potvrdom identiteta.

Pogodnosti: Proaktivna potvrda identiteta omogućava potvrdu identiteta ključnim uslugama, kao što je Kancelarija Stranica nove kartice. Takođe, ako se Bing koristi kao pretraživač, Proaktivna potvrda identiteta poboljšava performanse trake adresa i pomaže u generisanju rezultata pretrage personalizovanih prema potrebama vašeg preduzeća.

**Windows Hello CredUI za NTLM potvrdu identiteta**

Ako jedinstveno prijavljivanje (SSO) nije dostupno kada veb sajt pokuša da se prijavi na korisnika putem NTLM ili Negotiate mehanizma, ova funkcija će omogućiti korisniku da deli OS akredicije sa veb lokacijom i da zadovolji izazov potvrde identiteta korišćenjem cred korisničkog interfejsa Windows Hello Cred UI. Ovaj tok prijavljivanje će se pojaviti samo u Windows 10 i samo za korisnike koji ne dobijaju SSO tokom NTLM-a ili sporazumnog izazova.

**Korišćenje sačuvanih lozinki za automatsko prijavljivanje**

Korisnici koji čuvaju lozinke Microsoft Edge mogu da omoguće automatsko prijavljivanje na veb lokacije na kojima imaju sačuvane akredicije. Korisnici mogu da uključe ili isključe ovu funkciju edge://settings/passwords, a vi možete da je konfigurišete u [smernicama menadžera lozinki.](https://go.microsoft.com/fwlink/?linkid=2134622)
