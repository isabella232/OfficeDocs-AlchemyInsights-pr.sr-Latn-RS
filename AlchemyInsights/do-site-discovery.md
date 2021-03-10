---
title: Otkrivanje lokacija
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
ms.openlocfilehash: bdf94220de45d92f63e56501ea4e35389224d25c
ms.sourcegitcommit: 475a9eaa095812091991857df6cf6490a8bbe179
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/08/2021
ms.locfileid: "50694559"
---
# <a name="do-site-discovery"></a>Otkrivanje lokacija

Ako organizacija i dalje koristi zastarele Veb aplikacije i planove za korišćenje programa Internet Explorer (koje većina klijenata ima), trebalo bi da uradite nešto dodatno otkrivanje lokacije.

**Već ste rasporedili stariju verziju Microsoft Edge**

Ako ste već konfigurisali listu preduzeća da radi za nasleđenu verziju sistema Microsoft Edge, otkrivanje lokacije će biti gotovo gotovo. Jedina stvar koju treba da uradite je da dodate neutralne lokacije.

Neutralne lokacije najčešće su lokacije koje pružaju jedinstveno prijavljivanje (SSO). Ako odete na neutralnu lokaciju sa lokacije Microsoft Edge, želite da ostanete u aplikaciji Microsoft Edge da biste se potvrdili autentičnosti. Ako odete na neutralnu stranicu u režimu programa Internet Explorer, zatim želite da ostanete u režimu programa Internet Explorer da biste potvrdili autentičnost.

Identifikujte SSO ili druge neutralne lokacije koje koristite i dodajte ih na listu poslovnih lokacija.

**Internet Explorer je podrazumevani pregledač**

Ako sada koristite samo Internet Explorer, možda ne znate koje su lokacije nadograđene na moderne Veb standarde i koje i dalje zahtevaju Internet Explorer. Ove lokacije ćete želeti da pronađete i dodate na listu lokacije preduzeća kako biste mogli da koristite Internet Explorer samo za te lokacije.

> [!NOTE]
> [Otkrivanje lokacije preduzeća](https://docs.microsoft.com/internet-explorer/ie11-deploy-guide/collect-data-using-enterprise-site-discovery) otkriva lokacije kojima je možda potreban Internet Explorer režim. Možete prikupiti podatke na računarima koji rade pod operativnim sistemom Windows Internet Explorer 8 putem Internet Explorer 11 u operativnom sistemu Windows 10, Windows 8,1 ili Windows 7.

**Analiza podataka**

Pošto ste prikupili podatke na sajtu, preporučujemo da sledeći proces iz četiri koraka analizira podatke:
1. Sortirajte podatke po domenu, a zatim po URL adresi.
2. Definišite granice aplikacije za konfiguraciju za Internet Explorer režim. Želite da dodate sve lokacije i Veb kontrole koje definišu aplikaciju, ali ne želite da dodate dodatne lokacije i kontrole. Neke lokacije mogu biti jednostavne kao i *https://contoso.com/app1* dok će drugi možda zahtevati da definišete više sajtova i stranica.
3. Testirate aplikaciju da biste proverili da li izvorno radi. Mnoge lokacije će ponuditi moderan sadržaj kada otkriju moderni pregledač i ponude zastareli sadržaj samo kada otkriju Internet Explorer.
4. Dodajte aplikaciju na listu poslovnih lokacija ako ne uspe da testira.

> [!NOTE]
> Kao najbolju praksu, grupišete sve lokacije koje sačinjavaju aplikaciju. Na ovaj način, kada nadogradite aplikaciju, možete lakše da uklonite celu stranicu iz režima programa Internet Explorer i počnete da koristite moderan pregledač za tu aplikaciju.

Kada završite sa otkrivanjem sajta i analizirajte podatke, spremni ste da počnete da tražite strategiju kanala.

