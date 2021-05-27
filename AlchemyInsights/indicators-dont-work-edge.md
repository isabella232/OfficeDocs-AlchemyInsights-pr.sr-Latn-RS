---
title: Indikatori ne rade pomoću pregledača Edge
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11230"
- "9005470"
ms.openlocfilehash: df62d965e0dc2ddb656571af99b1e4c3cb52ea35
ms.sourcegitcommit: 4b504650e11adb9894c37b6d8608b53f9d5fc13d
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 05/25/2021
ms.locfileid: "52676465"
---
# <a name="indicators-dont-work-using-edge-browser"></a>Indikatori ne rade pomoću pregledača Edge

Kada kreirate indikator, Edge (Smartscreen) ga ne poštuje. Dodatne informacije potražite u [temi Pravljenje indikatora za IP-ove i UL-ove/domene.](/microsoft-365/security/defender-endpoint/indicator-ip-domain)

## <a name="step-1-ensure-the-following"></a>1. korak: Obezbedite sledeće

- Proverite da li je indikator ispravan (nema greške u greškama u IP/URL adresi, odgovarajuća radnja, odgovarajuće RBAC grupe).
- Sačekajte najmanje 2 časa nakon kreiranja indikatora da biste uzeti u obzir eventualna kašnjenja.
- Potvrdite da su sistemi spremni za microsoft zaštitnik za krajnje tačke.
- Potvrdite da sistemi mogu da komuniciraju sa oblakom.
- Uverite se da je Smartscreen omogućen i da može da mu se pristupi tako što ćete ići na [sajt za testiranje.](https://demo.smartscreen.msft.net)

## <a name="step-2-troubleshoot-the-potential-issue"></a>2. korak: Rešavanje potencijalnog problema

- Proverite da li klijent ispunjava zahteve. Za detalje pogledajte Kreiranje [indikatora za IP-ove i UL-ove/domene.](/microsoft-365/security/defender-endpoint/indicator-ip-domain)
- Proverite da li imate najnoviju verziju pregledača Edge. Da biste videli najnoviju verziju, pogledajte [saznajte koju verziju sistema Microsoft Edge imate.](https://support.microsoft.com/microsoft-edge/find-out-which-version-of-microsoft-edge-you-have-c726bee8-c42e-e472-e954-4cf5123497eb)
- Ponovo pokrenite pregledač Edge.
- Odete na sajt za koji ste instalirali indikator. Ako se lokacija ne pojavi na očekivani način, pređite na 3. korak. 

## <a name="step-3-collect-data"></a>3. korak: Prikupljanje podataka

- Prikupljanje **dijagnostičkih podataka za MDEClientAnalyzer.** Uputstva možete da [vidite u članku Problemi sa mašinama za uletanje u Microsoft zaštitnik za krajnju tačku.](issues-with-onboarding-machines.md)
- Ako vam je udobno da instalirate i prikupljate Fiddler praćenje, pogledajte [telerik Fiddler](http://www.telerik.com/fiddler).
- Ako želite uputstva od Microsoft podrške, kliknite na ikonu Podrška ispod da biste otvorili predmet podrške.
