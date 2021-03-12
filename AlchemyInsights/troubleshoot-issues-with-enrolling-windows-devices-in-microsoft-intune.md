---
title: Rešavanje problema sa ugrađenim Windows uređajima u Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: 88105671ef6dc34553a265937bf1fb3463353963
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708904"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>Rešavanje problema sa ugrađenim Windows uređajima u Microsoft Intune

Pregledajte resurse navedene ispod da biste odmah rešili problem.
  
Neke uobičajene poruke o greškama i korake rezolucije:
  
 **Nije moguće instalirati softver, 0x80cf4017:** Certifikat naloga je istekao. Ponovo preuzmite softver klijenta klijenta u konzoli administracije Intune. Pregledajte ovu dokumentaciju za više informacija.
  
 **Kôd greške 0x801c0003:** Greška može da se pojavi u sledećim slučajevima:
  
-  Korisnik ima više uređaja upisano od ograničenja uređaja. Pregledajte ove dokumente da [biste uklonili uređaj](https://docs.microsoft.com/intune/devices-wipe) ili [promenili ograničenje uređaja](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).

-  "Korisnici mogu da pridruže uređajima na Azure AD" podešeno je na "nijedno". Postavljanje na sve ili izbor korisnika. Pregledajte [ovu dokumentaciju](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) za više informacija.

-  Uređaj je već upisan od strane drugog korisnika. Ako je to slučaj, uklonite uređaj iz Azure Intune konzole ili ručno opozovite uređaj pre nego što pokušate ponovo.

-  Uređaj je Windows 10 Home. Samo Windows 10 pro, obrazovanje i Enterprise MJ mogu da se pridruže Azure aktivnom direktorijumu.

Dodatni resursi koji će vam pomoći da rešite problem:
  
-  Koristite [portal za rešavanje problema sa Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) da biste dijagnostikovali i rešili uobičajene greške unosa. Pregledajte [ovaj dokument](https://docs.microsoft.com/intune/help-desk-operators) za više detalja.

-  Redigujte ove dokumente za listu uobičajenih grešaka koje mogu da se prijave i rešenja za svaki: [Vodič za rešavanje problema](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) i [Rešavanje problema sa doktorom](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).

[Saznajte kako da Upisite Windows uređaje u Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).
