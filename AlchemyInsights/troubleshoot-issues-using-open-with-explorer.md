---
title: Rešavanje problema pri korišćenju funkcije "Otvaranje pomoću programa Explorer"
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
ms.assetid: ed852342-e33f-4450-8400-63d30df09476
ms.openlocfilehash: 49d6d449af6e718d70c9948a03f7e2e1e21517d2
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/13/2021
ms.locfileid: "58323580"
---
# <a name="fix-problems-with-open-with-explorer"></a>Rešavanje problema sa programom Explorer

Rešite uobičajene probleme sa otvaranjem biblioteke dokumenata SharePoint ili OneDrive **komande Otvori pomoću programa Explorer:** 
  
- Koristite Internet Explorer 10 ili Internet Explorer 11. **Postavka Otvori** uz Explorer nije kompatibilna sa programima Microsoft Edge, Google Chrome, Firefox i drugim. **Postavka Otvori u** programu Explorer je onemogućena u svim pregledačima osim u programu Internet Explorer. 
    
- **Postavka Otvori** u programu Explorer nije dostupna u modernom iskustvu SharePoint bibliotekama. Umesto toga **koristite prikaži u istraživaču** datoteka. Izaberite **stavku Prikaz opcija Prikaz** u \> **istraživaču datoteka**. Prikaz u istraživaču datoteka nije kompatibilan sa programima Microsoft Edge, Google Chrome, Firefox i drugim. **Prikažite u istraživaču datoteka u** dostupnim samo u programu Internet Explorer. 
    
- Uverite se da je usluga WebClient pokrenuta. U polju Windows otkucajte pokreni, izaberite aplikaciju za računare Pokreni, otkucajte services.msc, a zatim pritisnite taster Enter. Pomerite se nadole do usluge WebClient i uverite se da **kolona Status** prikazuje "Pokrenuto". Ako se to ne ukaže, kliknite dvaput na uslugu, izaberite stavku **Start**, a zatim kliknite na dugme **U redu.** (Možda ćete prvo morati da omogućite uslugu tako što ćete izabrati stavku **Ručno** ili **Automatsko** u polju Tip **pokretanja.)** 
    
**Na primer:** Otvaranje biblioteke u istraživaču datoteka je pri ruci ako treba da kopirate ili premestite više datoteka i fascikli jednom, ali ako želite redovno da radite u biblioteci, preporučujemo da je sinhronizujete. Da biste rešili probleme sa otvaranjem u istraživaču datoteka, pogledajte [otvaranje u programu Explorer.](https://go.microsoft.com/fwlink/?linkid=871665) Informacije o podešavanju sinhronizacije potražite u [SharePoint Sinhronizacija datoteka pomoću novog OneDrive aplikacija za sinhronizaciju klijenta.](https://go.microsoft.com/fwlink/?linkid=871666)
  
Više informacija potražite u [članku Korišćenje komande "Otvori pomoću programa Explorer"](https://docs.microsoft.com/sharepoint/support/lists-and-libraries/troubleshoot-issues-using-open-with-explorer) za rešavanje problema u programu SharePoint Online. 
  

