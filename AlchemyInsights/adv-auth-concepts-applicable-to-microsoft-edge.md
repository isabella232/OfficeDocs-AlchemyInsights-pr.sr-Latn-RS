---
title: Napredni koncepti autentičnosti primenljiv na Microsoft Edge
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
ms.openlocfilehash: 241d594fac6664dd1e85fd60e30a6344c432555e
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573529"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a>Napredni koncepti autentičnosti primenljiv na Microsoft Edge

Slede Napredni koncepti autentičnosti koji se primenjuju na Microsoft Edge:

**Proaktivna potvrda identiteta**

Kada omogućite smernice za [Proactiveda](https://go.microsoft.com/fwlink/?linkid=2134621) , Microsoft Edge će pokušati da produzi potvrdu o prijavljivanju korisnika u Microsoft usluge. U redovnim intervalima, ona će koristiti uslugu na mreži za proveru ažuriranog manifesta koji sadrži trenutnu potvrdu konfiguracije.

Beneficije: proaktivna potvrda identiteta omogućava potvrdu identiteta na ključnim uslugama, kao što je stranica Office nova kartica. Takođe, ako se Bing koristi kao pretraživač, proaktivna potvrda identiteta poboljšava performanse trake adresa i pomaže pri generisanje rezultata pretrage personalizovanih na potrebe preduzeća.

**Windows Hello Kredui za NTLM potvrdu identiteta**

Ako je pojedinačni prijavljivanje (SSO) nije dostupan kada Veb lokacija pokuša da se prijavi na korisnika kroz NTLM ili pregovaranje mehanizma, ova funkcija će korisniku omogućiti da deli akreditive OS sa Veb lokacijom i da bi ispunila izazov potvrde identiteta pomoću Windows Hello Ccrveni UI. Ovaj tok prijavljivanja pojaviće se samo u operativnom sistemu Windows 10 i samo za korisnike koji ne primaju SSO tokom NTLM ili pregovaranja.

**Korišćenje sačuvanih lozinki za automatsko prijavljivanje**

Korisnici koji čuvaju lozinke u aplikaciji Microsoft Edge mogu da omoguću automatsko prijavljivanje na Veb lokacije na kojima imaju sačuvane akreditive. Korisnici mogu da uključe ovu funkciju u edge://settings/passwords i da je konfigurišete u smernicama [upravljača lozinkama](https://go.microsoft.com/fwlink/?linkid=2134622) .
