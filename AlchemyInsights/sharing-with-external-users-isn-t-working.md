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
ms.openlocfilehash: bd3a6c0d7206801ff76be121c4878b8343cc9886
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47691589"
---
# <a name="fix-problems-sharing-sharepoint-content-with-external-users"></a>Rešavanje problema deljenja SharePoint sadržaja sa spoljnim korisnicima

Uverite se da je spoljašnje deljenje uključeno za vašu organizaciju:
  
1. Idite na [ &amp; stranicu programski dodaci usluge u Microsoft 365 centru administracije](https://portal.office.com/adminportal/home#/Settings/ServicesAndAddIns)i izaberite stavku **lokacije**.
    
2. Proverite da li je postavka uključena u "uključeno". Ako je izabrana stavka "samo postojeći spoljni korisnici", uverite se da je spoljni korisnik naveden u Microsoft 365 centru administracije.
    
Proverite da li je spoljni deljenje uključeno za sajt. Za klasičnu kolekciju lokacija:
  
1. U novom SharePoint centru administracije, u levom oknu izaberite stavku **lokacije**.
    
2. Izaberite lokaciju ili lokacije i na traci kliknite na dugme **Deljenje**.
    
Za lokaciju tima koja pripada Microsoft 365 grupi ili na lokaciji za komunikaciju:
  
- Ovi novi tipovi lokacija imaju istu postavku deljenja kao i postavka za celu organizaciju, osim ako postavka za celu organizaciju ne omogućava deljenje datoteka pomoću veza koje ne zahteva prijavljivanje. U ovom slučaju, lokacije omogućava deljenje sa novim i postojećim spoljnim korisnicima koji se prijave. Da biste promenili postavku za određene lokacije, koristite novi SharePoint centar administracije ili PowerShell. [Saznajte više](https://go.microsoft.com/fwlink/?linkid=871863).
    
> [!NOTE]
> Postavke spoljnog deljenja za bilo koju stranicu mogu da budu restriktivnije od vaše postavke za celu organizaciju, ali ne i više od toga. 
  

