---
title: Rešavanje problema sa upisivanju Android uređaja u Microsoft Intune
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
ms.openlocfilehash: 0ae926e6b31493e7359981c621fd27e8f53d49a17bdf107173b087fe6cc688fa
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "54008092"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>Rešavanje problema sa upisivanju Android uređaja u Microsoft Intune

Pregledajte resurse navedene ispod da biste odmah rešili problem.
  
Neki uobičajeni problemi i koraci za rešavanje problema:
  
 **Greška "Uređaj nije šifrovan" u Company Portal:** Novije verzije operativnog sistema Android, naročito verzije v7.0, zahtevaju pokreni kod da biste se uverili da je uređaj potpuno šifrovan. Uobičajena rešenja su omogućavanje PIN koda za pokretanje ili potpunog šifrovanja uređaja. Pregledajte [ovaj dokument](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) za više informacija.
  
 Uređaji ne uspevaju da se prijavite pomoću usluge Intune ili da se prikažu kao **"Neispravan" na Intune kontrolnoj konzoli:** Neki Samsung 4.4 i 5.5 uređaji možda neće prijaviti uslugu. Postoje 3 moguća rešenja za ovaj problem:
  
1. Ručno otvorite aplikaciju Intune Company Portal, što će automatski pokrenuti sinhronizaciju uređaja.

2. Ažurirajte uređaj na Android 6.0 ili noviju.

3. Onemogućite samsung Smart Manager da upravlja Intune Company Portal. Pregledajte [ovaj dokument](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) za više detalja o ovim problemima i rešenjima.

 **Greška "Tip korisničke licence** je nevažeći" ili "Nije prepoznato korisničko **ime":** Korisniku treba da bude dodeljena Intune ili EMS licenca. Pregledajte ove dokumente da biste dodelili licencu preko: Kancelarija centra za Kancelarija ili Azure portala.
  
Dodatni resursi koji vam pomažu da rešite problem:
  
1. Koristite [Intune portal za rešavanje problema da](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) biste dijagnostikovali i rešili uobičajene greške u vezi sa unošenjem. Pregledajte [ovaj dokument](https://docs.microsoft.com/intune/help-desk-operators) za više detalja.

2. Pregledajte [ovaj](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) dokument da biste videli listu uobičajenih grešaka koje sprečavaju unošenje i rešenja za svaku od njih.

3. [Saznajte kako da uklonite Android uređaje u aplikaciju Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).
