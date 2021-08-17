---
title: Deljenje sa spoljnim korisnicima ne funkcioniše
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: 02d79c1b1e112eb41e8c60ffa2ef28e429f76ada
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/13/2021
ms.locfileid: "58304383"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a>Rešavanje problema sa deljenjem SharePoint sa spoljnim korisnicima

Uverite se da je spoljno deljenje uključeno za organizaciju:
  
1. Idite na [stranicu &amp; "Programski dodaci za Usluge" u Microsoft 365 centar administracije](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns)i izaberite stavku **Lokacije.**
    
2. Uverite se da je postavka uključena na "Uključeno". Ako je izabrana stavka "Samo postojeći spoljni korisnici", proverite da li je spoljni korisnik naveden u Microsoft 365 centar administracije.
    
Uverite se da je spoljno deljenje uključeno za lokaciju. Za klasičnu kolekciju sajtova:
  
1. U novom SharePoint za administovanje, u levom oknu izaberite stavku **sajtovi**.
    
2. Izaberite sajt ili sajtove i na traci izaberite stavku **Deljenje**.
    
Za sajt tima koji pripada Microsoft 365 grupi ili sajtu za komunikaciju:
  
- Ovi novi tipovi sajtova imaju istu postavku deljenja kao i postavka na celom sajtu organizacije, osim ako postavka na celom sajtu organizacije ne dozvoljava deljenje datoteka pomoću veza koje ne zahtevaju prijavljivanje. U tom slučaju, sajtovi omogućavaju deljenje sa novim i postojećim spoljnim korisnicima koji se prijavljuju. Da biste promenili postavku za određene sajtove, koristite novi SharePoint ili PowerShell. [Saznajte više](https://go.microsoft.com/fwlink/?linkid=871863).
    
Napom: Postavka spoljnog deljenja za bilo koju lokaciju može da bude restriktivniji od postavke na celom sajtu **organizacije,** ali ne može da ima veću upotrebu od postavke na celom sajtu organizacije. 
  

