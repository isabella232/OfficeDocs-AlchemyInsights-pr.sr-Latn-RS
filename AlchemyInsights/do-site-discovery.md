---
title: Otkrivanje sajta
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9143"
- "9005291"
ms.openlocfilehash: 4653fdef7e9226f05809d56e9a445cd1da35b0578c088bea72252a281d4527d2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "54030772"
---
# <a name="do-site-discovery"></a>Otkrivanje sajta

Ako vaša organizacija i dalje koristi zakasnele veb aplikacije i planove za korišćenje režima pregledača Internet Explorer (što radi većina korisnika), trebalo bi da uradite neko dodatno otkrivanje sajta.

**Već ste primenili stariju verziju programa Microsoft Edge**

Ako ste već konfigurisali listu sajtova preduzeća da radi za zatamnjenu verziju usluge Microsoft Edge, otkrivanje sajta je skoro gotovo. Trebalo bi da dodate neutralne sajtove.

Neutralni sajtovi su obično sajtovi koji obezbeđuju jedinstveno prijavljivanje (SSO). Ako odete na neutralni sajt iz usluge Microsoft Edge, onda želite da ostanete u Microsoft Edge biste potvrdili identitet. Ako odete na neutralnu lokaciju u režimu pregledača Internet Explorer, želite da ostanete u režimu pregledača Internet Explorer da biste potvrdili identitet.

Identifikujte sve SSO ili druge neutralne sajtove koje koristite i dodajte ih na listu lokacija preduzeća.

**Internet Explorer je podrazumevani pregledač**

Ako sada samo koristite Internet Explorer, možda ne znate koje lokacije su izvršile nadogradnju na moderne veb standarde i koje i dalje zahtevaju Internet Explorer. Te lokacije ćete želeti da pronađete i dodate na listu sajtova preduzeća kako biste mogli da koristite režim pregledača Internet Explorer samo za te lokacije.

> [!NOTE]
> [Otkrivanje sajtova preduzeća](https://docs.microsoft.com/internet-explorer/ie11-deploy-guide/collect-data-using-enterprise-site-discovery) otkriva sajtove koji su možda potrebni režimu programa Internet Explorer. On može da prikuplja podatke na računarima koji koriste Windows Internet Explorer 8 kroz Internet Explorer 11 na Windows 10, Windows 8.1 ili Windows 7.

**Analiziranje podataka**

Kada prikupite podatke sajta, preporučujemo vam da analizirate podatke u četiri koraka:
1. Sortirajte podatke po domenu, a zatim po URL adresi.
2. Definišite granice aplikacije da biste konfigurisali režim programa Internet Explorer. Želite da uključite sve lokacije i veb kontrole koje definišu aplikaciju, ali ne želite da uključite dodatne lokacije i kontrole. Neki sajtovi mogu biti jednostavni, *https://contoso.com/app1* dok drugi mogu zahtevati da definišete više sajtova i stranica.
3. Testirajte aplikaciju da biste potvrdili da ona ne radi kako treba. Mnogi sajtovi će ponuditi moderan sadržaj kada otkriju moderan pregledač i nude zatamnjeni sadržaj samo kada otkriju Internet Explorer.
4. Dodajte aplikaciju na listu lokacije preduzeća ako testiranje ne uspe.

> [!NOTE]
> Kao najbolju praksu, grupišite sve lokacije koje se sastoje od aplikacije. Na taj način ćete lakše ukloniti celu lokaciju iz režima pregledača Internet Explorer i početi da koristite moderan pregledač za tu aplikaciju.

Kada završite sa otkrivanjem sajta i analizirate podatke, spremni ste da počnete da gledate strategiju kanala.

