---
title: Rešavanje problema sa enkotrljnim Windows uređajima u usluzi Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: 7b298360fe31d3f52ef382e5b8f25ee3588c36c8
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 06/02/2020
ms.locfileid: "36665846"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>Rešavanje problema sa enkotrljnim Windows uređajima u usluzi Microsoft Intune

Pregledajte dole navedene resurse da biste odmah rešili problem.
  
Neke uobičajene poruke o grešci i koraci rešenja:
  
 **Softver ne može biti instaliran, 0x80cf4017:** Vaš certifikat naloga je istekao. Ponovo preuzmite paket za klijentski softver računara u usluzi Intune admin Console. Pregledajte ovu dokumentaciju za više informacija.
  
 **Kôd greške 0x801c0003:** Do greške može doći u sledećim slučajevima:
  
-  Korisnik je više uređaja upisalo od ograničenja uređaja. Pregledajte ove dokumente da biste [uklonili uređaj](https://docs.microsoft.com/intune/devices-wipe) ili [promenili ograničenje uređaja](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).

-  "Korisnici se mogu pridružiti uređajima za Azure oglas" podešeni su na "nijedan". Postavite ga na sve ili izaberite korisnike. Pregledajte [ovu dokumentaciju](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) za više informacija.

-  Uređaj već upisuje drugi korisnik. Ako je to slučaj, uklonite uređaj sa Azure Intune konzole ili ručno deprijavite uređaj pre nego što ponovo pokušate.

-  Uređaj je Windows 10 Home. Samo Windows 10 pro, obrazovanje i Enterprise SKUs mogu da pristupe Azure aktivnom direktorijumu.

Dodatni resursi koji vam pomažu da rešite problem:
  
-  Koristite [Intune za rešavanje problema](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) da biste ustanovili i rešili uobičajene greške u uvrštavanju. Pregledajte [ovaj dokument](https://docs.microsoft.com/intune/help-desk-operators) za više detalja.

-  Pregledajte ove dokumente da biste dobili listu uobičajenih grešaka koje sprečavaju upis i rešenja za svaki: [Vodič za rešavanje problema](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) i [Rešavanje problema sa programom Doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).

[Saznajte kako da prijavite Windows uređaje u programu Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).
