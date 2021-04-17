---
title: Rešavanje problema sa upisivanju Android uređaja u aplikaciji Microsoft Intune
ms.author: pebaum
author: pebaum
manager: scotv
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
ms.openlocfilehash: 08620a44dcf693482c65ff05e19f11870f67afbe
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830956"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>Rešavanje problema sa upisivanju Android uređaja u aplikaciji Microsoft Intune

Pregledajte resurse navedene ispod da biste odmah rešili problem.
  
Neki uobičajeni problemi i koraci za rešavanje problema:
  
 **Greška "Uređaj nije šifrovan" na portalu preduzeća:** Novije verzije operativnog sistema Android, naročito verzije v7.0, zahtevaju pokreni kod da biste se uverili da je uređaj potpuno šifrovan. Uobičajena rešenja su omogućavanje PIN koda za pokretanje ili potpunog šifrovanja uređaja. Pregledajte [ovaj dokument](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) za više informacija.
  
 Uređaji ne uspevaju da se prijavite pomoću usluge Intune ili da se prikažu kao **"Neispravan" na Intune kontrolnoj konzoli:** Neki Samsung 4.4 i 5.5 uređaji možda neće prijaviti uslugu. Postoje 3 moguća rešenja za ovaj problem:
  
1. Ručno otvorite aplikaciju Intune Company Portal, koja će automatski pokrenuti sinhronizaciju uređaja.

2. Ažurirajte uređaj na Android 6.0 ili noviju.

3. Onemogućite samsung Smart Manager da upravlja intune Company Portalom. Pregledajte [ovaj dokument](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) za više detalja o ovim problemima i rešenjima.

 **Greška "Tip korisničke licence** je nevažeći" ili "Nije prepoznato korisničko **ime":** Korisniku treba da bude dodeljena Intune ili EMS licenca. Pregledajte ove dokumente da biste dodelili licencu preko: Office centra za administarcije ili Azure portala.
  
Dodatni resursi koji vam pomažu da rešite problem:
  
1. Koristite [Intune portal za rešavanje problema da](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) biste dijagnostikovali i rešili uobičajene greške u vezi sa unošenjem. Pregledajte [ovaj dokument](https://docs.microsoft.com/intune/help-desk-operators) za više detalja.

2. Pregledajte [ovaj](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) dokument da biste videli listu uobičajenih grešaka koje sprečavaju unošenje i rešenja za svaku od njih.

3. [Saznajte kako da uklonite Android uređaje u aplikaciju Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).
