---
title: Rešavanje problema sa upisivanju iOS uređaja u aplikaciju Microsoft Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 14f7a897f0c7504db1b605485e170183c3a1afb2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/15/2021
ms.locfileid: "51823477"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>Rešavanje problema sa upisivanju iOS uređaja u aplikaciju Microsoft Intune

Pregledajte resurse navedene ispod da biste odmah rešili problem. 
  
Neke uobičajene poruke o grešci i koraci za rešavanje problema:
  
- **Dostignuto je capava uređaja** Korisnik je upisan više uređaja nego što je ograničenje uređaja. Pregledajte ove dokumente da [biste uklonili uređaj](https://docs.microsoft.com/intune/devices-wipe) [ili promenili ograničenje uređaja.](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)
    
- **Ova usluga nije podržana. Nema smernica za unošenje:** Apple usluga push obaveštenja (APNS) treba da se konfiguriše ili obnovi. Pregledajte [ovaj dokument](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) da biste pregledali uputstva kako da to uradite. 
    
- **Tip korisničke licence nevažeći ili korisničko ime nije prepoznato:** Korisniku mora da bude dodeljena Intune ili EMS licenca. Pregledajte ove dokumente da biste dodelili licencu preko: [Office centra za administarcije](https://docs.microsoft.com/intune/licenses-assign) ili [Azure portala.](https://docs.microsoft.com/azure/active-directory/license-users-groups)
    
Dodatni resursi koji vam pomažu da rešite problem:
  
1. Koristite [Intune portal za rešavanje problema da](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) biste dijagnostikovali i rešili uobičajene greške u vezi sa unošenjem. Pregledajte [ovaj dokument](https://docs.microsoft.com/intune/help-desk-operators) za više detalja. 
    
2. Pregledajte ove dokumente da biste videli listu uobičajenih grešaka koje sprečavaju unošenje i rešenja za svaki [od](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) njih: Vodič za rešavanje problema i dokument za [rešavanje problema.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)
    
3. [Saznajte kako da uredite iOS uređaje u aplikaciji Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).
    

