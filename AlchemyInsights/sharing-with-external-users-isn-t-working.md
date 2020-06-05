---
title: Deljenje sa spoljnim korisnicima ne radi
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: d3d0b69b-214e-4859-8957-621fd6306b30
ms.openlocfilehash: 9a40f52637bc8aa7894754118f0f862aa6c71fe2
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 06/05/2020
ms.locfileid: "44582789"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a>Rešavanje problema sa deljenjem SharePoint sadržaja sa spoljnim korisnicima

Proverite da li je uključeno zajedničko deljenje za vašu organizaciju:
  
1. Idite na [stranicu " &amp; programski dodaci za usluge" u Microsoft 365 admin Center](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns)i izaberite stavku **lokacije**.
    
2. Proverite da li je postavka uključena u "uključeno". Ako je izabrano "samo postojeći spoljni korisnici", uverite se da je spoljni korisnik naveden u Microsoft 365 admin Center.
    
Uverite se da je spoljna podela uključena za lokaciju. Za klasičnu kolekciju lokacija:
  
1. U novom SharePoint administratoru centra, u levom oknu izaberite stavku **lokacije**.
    
2. Izaberite lokaciju ili lokacije i na glavnoj traci kliknite na dugme **Deljenje**.
    
Za lokaciju tima koja pripada Microsoft 365 grupi ili lokaciji za komunikaciju:
  
- Ovi novi tipovi lokacija imaju istu postavku deljenja kao i postavke za celu organizaciju, osim ako postavka za celu organizaciju ne dozvoljava deljenje datoteka pomoću veza koje ne zahtevaju prijavljivanje. U ovom slučaju, lokacije omogućavaju deljenje sa novim i postojećim spoljnim korisnicima koji se prijave. Da biste promenili postavke za određene lokacije, koristite novi SharePoint admin Center ili PowerShell. [Saznajte više](https://go.microsoft.com/fwlink/?linkid=871863).
    
> [!NOTE]
> Postavka spoljnog deljenja za svaku lokaciju može da bude restriktivnija od postavke za celu organizaciju, ali ne i veća od postavke za celu organizaciju. 
  

