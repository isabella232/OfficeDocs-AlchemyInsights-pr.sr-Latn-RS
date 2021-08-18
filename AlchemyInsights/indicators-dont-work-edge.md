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
ms.openlocfilehash: 2a48a49ec52a585e450edf448bc9203cd9c3f935
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/13/2021
ms.locfileid: "58326275"
---
# <a name="indicators-dont-work-using-edge-browser"></a>Indikatori ne rade pomoću pregledača Edge

Kada kreirate indikator, Edge (Smartscreen) ga ne poštuje. Dodatne informacije potražite u [temi Pravljenje indikatora za IP-ove i UL-ove/domene.](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/indicator-ip-domain)

## <a name="step-1-ensure-the-following"></a>1. korak: Obezbedite sledeće

- Proverite da li je indikator ispravan (nema greške u greškama u IP/URL adresi, odgovarajuća radnja, odgovarajuće RBAC grupe).
- Sačekajte najmanje 2 časa nakon što kreirate indikator uzimajući u obzir eventualna kašnjenja.
- Potvrdite da su sistemi spremni za microsoft zaštitnik za krajnje tačke.
- Potvrdite da sistemi mogu da komuniciraju sa oblakom.
- Uverite se da je Smartscreen omogućen i da može da mu se pristupi tako što ćete ići na [sajt za testiranje.](https://demo.smartscreen.msft.net)

## <a name="step-2-troubleshoot-the-potential-issue"></a>2. korak: Rešavanje potencijalnog problema

- Proverite da li klijent ispunjava zahteve. Za detalje pogledajte Kreiranje [indikatora za IP-ove i UL-ove/domene.](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/indicator-ip-domain)
- Proverite da li imate najnoviju verziju pregledača Edge. Da biste videli najnoviju verziju, pogledajte [saznajte koju verziju sistema Microsoft Edge imate.](https://support.microsoft.com/microsoft-edge/find-out-which-version-of-microsoft-edge-you-have-c726bee8-c42e-e472-e954-4cf5123497eb)
- Ponovo pokrenite pregledač Edge.
- Odete na sajt za koji ste instalirali indikator. Ako se lokacija ne pojavi na očekivani način, pređite na 3. korak. 

## <a name="step-3-collect-data"></a>3. korak: Prikupljanje podataka

- Prikupljanje **dijagnostičkih podataka za MDEClientAnalyzer.** Uputstva možete da [vidite u članku Problemi sa mašinama za uletanje u Microsoft zaštitnik za krajnju tačku.](issues-with-onboarding-machines.md)
- Ako vam je udobno da instalirate i prikupljate Fiddler praćenje, pogledajte [telerik Fiddler](http://www.telerik.com/fiddler).
- Ako želite uputstva od Microsoft podrške, kliknite na ikonu Podrška ispod da biste otvorili predmet podrške.
