---
title: Mikro kašnjenja ili ograničavanje u usluzi Exchange Online PowerShell
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "5106"
ms.openlocfilehash: 2fab21f76f455815979ae162c1ce8246ad5c297e
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/13/2021
ms.locfileid: "58314714"
---
# <a name="micro-delays-or-throttling-in-exchange-online-powershell"></a>Mikro kašnjenja ili ograničavanje u usluzi Exchange Online PowerShell

Možda ćete videti upozorenja „Primenjeno je mikro kašnjenje“ ili kašnjenja kada pokrenete skripte ili cmdlet komande u usluzi Exchange Online. Evo nekoliko predloga kako da rešite ovo:

- Pokrenite našu dijagnostiku da biste opustili PowerShell smernice za zakupca. Ovo rešenje će rešiti problem za većinu.
- Ako problem još uvek nije rešen, [koristite modul Exchange Online v2 PowerShell,](https://docs.microsoft.com/powershell/exchange/exchange-online/exchange-online-powershell-v2/exchange-online-powershell-v2?view=exchange-ps&preserve-view=true)koji obuhvata CMDlet komande koje su zasnovane na REST API-u i znatno su performantnije. Ovo može biti odlično rešenje za Get- CMDlet komande koje se često koriste.
- Ako treba da koristite CMDlet komande koje nisu pokrivene v2 modulom, pročitajte tj. Pokretanje [PowerShell cmdlet](https://techcommunity.microsoft.com/t5/exchange-team-blog/updated-running-powershell-cmdlets-for-large-numbers-of-users-in/ba-p/1000628#)komandi za veliki broj korisnika u programu Office 365 , koja govori o tome kako da zaobičete PowerShell ograničenja za ograničavanje u Exchange Online.
