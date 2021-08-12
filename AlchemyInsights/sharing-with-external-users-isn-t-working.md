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
ms.openlocfilehash: 53f6fd009d3dab3cd66d33d9cd248201219caa1605c7a4e7758a5a8d720f68c2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "53910380"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a>Rešavanje problema sa deljenjem SharePoint sadržaju sa spoljnim korisnicima

Uverite se da je spoljno deljenje uključeno za organizaciju:
  
1. Idite na [stranicu &amp; "Programski dodaci za Usluge" u Microsoft 365 centar administracije](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns)i izaberite stavku **Lokacije.**
    
2. Uverite se da je postavka uključena na "Uključeno". Ako je izabrana stavka "Samo postojeći spoljni korisnici", proverite da li je spoljni korisnik naveden u Microsoft 365 centar administracije.
    
Uverite se da je spoljno deljenje uključeno za sajt. Za klasičnu kolekciju sajtova:
  
1. U novom centru SharePoint, u levom oknu izaberite stavku **sajtovi.**
    
2. Izaberite sajt ili sajtove i na traci izaberite stavku **Deljenje**.
    
Za sajt tima koji pripada Microsoft 365 grupi ili sajtu za komunikaciju:
  
- Ovi novi tipovi sajtova imaju istu postavku deljenja kao i postavka na celom sajtu organizacije, osim ako postavka na celom sajtu organizacije ne dozvoljava deljenje datoteka pomoću veza koje ne zahtevaju prijavljivanje. U tom slučaju, sajtovi omogućavaju deljenje sa novim i postojećim spoljnim korisnicima koji se prijavljuju. Da biste promenili postavku za određene sajtove, koristite novi SharePoint ili PowerShell. [Saznajte više](https://go.microsoft.com/fwlink/?linkid=871863).
    
> [!NOTE]
> Postavka spoljnog deljenja za bilo koji sajt može da bude restriktivniji od postavke na celom sajtu organizacije, ali ne može da bude pristupačnija od postavke u celom organizaciji. 
  

