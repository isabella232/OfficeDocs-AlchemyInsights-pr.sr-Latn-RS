---
title: Pristup uslugama penzija
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9000356"
- "2009"
ms.assetid: ''
ms.openlocfilehash: 943066d5ac76c0630554ee724bbab9a94086fae4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47698696"
---
# <a name="access-services-retirement"></a>Pristup uslugama penzija

Kao što smo se prvobitno najavili u MC97576, u martu 2017 i nastavili smo da komuniciramo u prethodnim godišnjim uslugama za pristup. Sledeća faza u ovom procesu je uklanjanje Access Veb baza podataka koje koriste SharePoint liste kao osnovno skladište podataka.

**Kako to utiče na mene?**

Počevši od juna 2019, Zaustavićemo kreiranje novih Access baza podataka u sistemu SharePoint Online i isključiti uslugu i sve preostale aplikacije do aprila 2020.

**Šta treba da uradim da bih se pripremio za ovu promenu?**

Podstićemo vas da kreirate prelaz plan za Access Veb baze podataka organizacije. Administratori mogu da koriste [SharePoint Access skener aplikacija](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) da bi nabavili zalihe Access aplikacija koje lokacije koriste.

Postoji nekoliko načina za migraciju podataka iz Veb baze podataka:

- Uvoz u lokalnu Access bazu podataka (. ACCDB) ili Excel datoteku.
- Preporučujemo da istražimo Microsoft PowerApps kao alternativnu platformu za kreiranje nekodova Business Solutions za Veb i mobilne uređaje.