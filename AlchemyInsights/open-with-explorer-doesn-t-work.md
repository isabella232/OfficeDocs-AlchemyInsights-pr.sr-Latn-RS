---
title: Otvaranje u programu Explorer ne funkcioniše
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b8f07022-69fe-4112-a2f6-d3a6cedb966c
ms.openlocfilehash: 164d5fe8c992df825d1f52f19792e1623526c35c58ff2f1e1ab601fdcf5f0f53
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "54011350"
---
# <a name="open-with-explorer-isnt-working"></a>Otvaranje u programu Explorer ne funkcioniše

Ako **opcija Otvori u** programu Explorer ili Prikaži u istraživaču datoteka  ne funkcioniše, proverite da li je usluga WebClient postavljena na Opciju "Pokrenuto" tako što će pratiti korake u nastavku.  Na primer, otvaranje biblioteke SharePoint ili OneDrive dok usluga nije pokrenuta. 
  
1. U Windows pretragu otkucajte pokreni, izaberite aplikaciju za računare Pokreni, otkucajte services.msc, a zatim izaberite **stavku Unesite**.
    
2. Pomerite se nadole do usluge WebClient i pogledajte **kolonu Status.** Ako status usluge WebClient nije pokrenut **,** kliknite dvaput na uslugu, kliknite na dugme **Start**, a zatim na dugme U **redu.** Omogućite uslugu, ako je  potrebno,  tako što će u polju Tip pokretanja izabrati **opciju** Ručno ili Automatsko. 
    
> [!NOTE]
> Da biste rešili probleme sa otvaranjem u istraživaču datoteka, pogledajte [otvaranje u programu Explorer.](https://go.microsoft.com/fwlink/?linkid=871665) Istražite sinhronizaciju kao bolju [alternativu: SharePoint sinhronizovanje datoteka pomoću novog OneDrive aplikacija za sinhronizaciju klijenta.](https://go.microsoft.com/fwlink/?linkid=871666) 
  

