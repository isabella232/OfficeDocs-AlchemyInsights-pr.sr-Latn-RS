---
title: Penzionisanje Access usluga
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
ms.openlocfilehash: 32da879de230dc0ed99563ad881ab5b2479b8453933a127961a26d619e108ab9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "53938709"
---
# <a name="access-services-retirement"></a>Penzionisanje Access usluga

Kao što smo prvobitno objavili u MC97576, u martu 2017. i nastavili da komuniciramo tokom prošle Access usluge se poništi. Sledeća faza u ovom procesu biće uklanjanje Access veb baza podataka koje koriste SharePoint kao deo skladišta podataka.

**Kako to utiče na mene?**

Počev od juna 2019, prestaćemo da kreiramo nove Access baze podataka u usluzi SharePoint Online i da isključimo uslugu i sve preostale aplikacije do aprila 2020.

**Šta treba da uradim da bih se pripremio za ovu promenu?**

Podstičemo vas da napravite plan prelaza za Access veb baze podataka vaše organizacije. Da bi dobili popis Access aplikacija koje [koriste lokacije,](https://github.com/SharePoint/PnP-Tools/tree/master/Solutions/SharePoint.AccessApp.Scanner) SharePoint Access aplikacije mogu da koriste zalihe Access aplikacija.

Postoji nekoliko načina za migrvanje podataka Access veb baza podataka:

- Uvoz u lokalnu Access bazu podataka (. ACCDB) ili na Excel datoteku.
- Takođe preporučujemo da istražite ovaj Microsoft PowerApps kao alternativnu platformu kako biste kreirali poslovna rešenja bez kodova za veb i mobilne uređaje.