---
title: Rešavanje problema sa enrolling iOS uređajima u programu Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 4aef78e5921b789b532fecc99380da3274173bdb
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708976"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>Rešavanje problema sa enrolling iOS uređajima u programu Microsoft Intune

Pregledajte resurse navedene ispod da biste odmah rešili problem. 
  
Neke uobičajene poruke o greškama i korake rezolucije:
  
- **Vrh uređaja je dostigao** Korisnik ima više uređaja upisano od ograničenja uređaja. Pregledajte ove dokumente da [biste uklonili uređaj](https://docs.microsoft.com/intune/devices-wipe) ili [promenili ograničenje uređaja](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).
    
- **Ova usluga nije podržana. Nema smernica** za prijavljivanje: Apple usluga push obaveštenja (APNS) mora da se konfiguriše ili obnovi. Pregledajte [ovaj dokument](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) za uputstva o tome kako to da uradite. 
    
- **Tip licenciranja korisnika je nevažeći ili nije prepoznat:** Korisniku treba da se dodeli Intune ili EMS licenca. Pregledajte ove dokumente da biste dodelili licencu putem: [Office administracije centra](https://docs.microsoft.com/intune/licenses-assign) ili [Azure portala](https://docs.microsoft.com/azure/active-directory/license-users-groups).
    
Dodatni resursi koji će vam pomoći da rešite problem:
  
1. Koristite [portal za rešavanje problema sa Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) da biste dijagnostikovali i rešili uobičajene greške unosa. Pregledajte [ovaj dokument](https://docs.microsoft.com/intune/help-desk-operators) za više detalja. 
    
2. Redigujte ove dokumente za listu uobičajenih grešaka koje mogu da se prijave i rešenja za svaki: [Vodič za rešavanje problema](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) i [Rešavanje problema sa doktorom](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).
    
3. [Saznajte kako da Upisite iOS uređaje u Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).
    

