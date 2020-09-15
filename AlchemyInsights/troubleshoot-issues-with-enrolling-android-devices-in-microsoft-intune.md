---
title: Rešavanje problema sa ugrađenim Android uređajima u programu Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: b5cb2e8a76e8e7d91bd9cd8789ae1623a7f96579
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/14/2020
ms.locfileid: "47689968"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>Rešavanje problema sa ugrađenim Android uređajima u programu Microsoft Intune

Pregledajte resurse navedene ispod da biste odmah rešili problem.
  
Neke uobičajene korake i korake rezolucije:
  
 **Greška uređaja nije šifrovana na portalu preduzeća:** Novije verzije programa android, naročito počevši od programa v 7.0, zahtevaju kôd za pokretanje sistema da biste se uverili da je uređaj potpuno šifrovan. Uobičajena rešenja su da omogućite PIN za pokretanje ili u potpunosti šifrujete uređaj. Pregledajte [ovaj dokument](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) za više informacija.
  
 **Uređaji se ne mogu prijaviti pomoću usluge Intune ili prikazani kao "nezdravi" u konzoli administracije Intune:** Neki Samsung 4,4 i 5,5 uređaji se možda neće prijaviti u uslugu. Postoji 3 moguća rešenja za ovaj problem:
  
1. Ručno otvorite aplikaciju Intune Company, koja će automatski započeti sinhronizaciju uređaja.

2. Ažurirajte uređaj na Android 6,0 ili noviji.

3. Onemogućavanje Samsung pametnog menadžera iz upravljanja portalu Intune Company. Pregledajte [ovaj dokument](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) za dodatne detalje o ovim temama i rezolucijama.

 **Tip licenciranja korisnika je nevažeći** ili **korisničko ime nisu prepoznati grešku:** korisniku treba da se DODELI Intune ili Ems licenca. Pregledajte ove dokumente da biste dodelili licencu putem: Office administracije centra ili Azure portala.
  
Dodatni resursi koji će vam pomoći da rešite problem:
  
1. Koristite [portal za rešavanje problema sa Intune](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) da biste dijagnostikovali i rešili uobičajene greške unosa. Pregledajte [ovaj dokument](https://docs.microsoft.com/intune/help-desk-operators) za više detalja.

2. Pregledajte [ovaj dokument](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) za listu uobičajenih grešaka koje sprečavaju upis i rezoluciju na svaki.

3. [Saznajte kako da Upisite Android uređaje u Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).
