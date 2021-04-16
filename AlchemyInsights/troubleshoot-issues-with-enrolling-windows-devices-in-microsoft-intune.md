---
title: Rešavanje problema sa upisivanju Windows uređaja u aplikaciju Microsoft Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: a456cc8f2336e6b902de0b7873cb233f4b846140
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/15/2021
ms.locfileid: "51808985"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>Rešavanje problema sa upisivanju Windows uređaja u aplikaciju Microsoft Intune

Pregledajte resurse navedene ispod da biste odmah rešili problem.
  
Neke uobičajene poruke o grešci i koraci za rešavanje problema:
  
 **Softver nije moguće instalirati, a 0x80cf4017:** Certifikat naloga je istekao. Ponovo preuzmite softverski paket PC klijenta na Intune kontrolnoj konzoli. Pregledajte ovu dokumentaciju za više informacija.
  
 **Kôd greške 0x801c0003:** Greška može da se pojavi u sledećim scenarijima:
  
-  Korisnik je upisan više uređaja nego što je ograničenje uređaja. Pregledajte ove dokumente da [biste uklonili uređaj](https://docs.microsoft.com/intune/devices-wipe) [ili promenili ograničenje uređaja.](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)

-  "Korisnici mogu da se pridruže uređajima u Azure AD" postavljeno je na "nijedno". Podesite na sve korisnike ili ih izaberite. Pregledajte [ovu dokumentaciju](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) za više informacija.

-  Uređaj je već upisao drugi korisnik. Ako je to slučaj, uklonite uređaj sa Azure Intune konzole ili ručno uklonite uređaj pre nego što pokušajte ponovo.

-  Uređaj je Windows 10 Home. Samo Windows 10 Pro, Education i Enterprise SKU-i mogu da se pridruže Azure Active Directory.

Dodatni resursi koji vam pomažu da rešite problem:
  
-  Koristite [Intune portal za rešavanje problema da](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) biste dijagnostikovali i rešili uobičajene greške u vezi sa unošenjem. Pregledajte [ovaj dokument](https://docs.microsoft.com/intune/help-desk-operators) za više detalja.

-  Pregledajte ove dokumente da biste videli listu uobičajenih grešaka koje sprečavaju unošenje i rešenja za svaki [od](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) njih: Vodič za rešavanje problema i dokument za [rešavanje problema.](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)

[Saznajte kako da uredite Windows uređaje u aplikaciji Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).
