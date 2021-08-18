---
title: 2681 Simulator napada u Microsoft 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2681"
ms.assetid: ''
ms.openlocfilehash: f6e221cc82a1b707f6acc457cb78db743521d859
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/13/2021
ms.locfileid: "58325085"
---
# <a name="attack-simulator-in-microsoft-365"></a>Simulator napada u Microsoft 365

- Da li vam nedostaje Simulator napada? Simulator napada zahteva **Microsoft zaštitnik za Office 365 Plan 2** **ili Office 365 Enterprise E5.** Simulator napada  nije uključen u Microsoft zaštitnik za Office 365 Plan 1, Office 365 Enterprise E3 ili bilo koje Microsoft 365 aplikacije za posao pretplate.

- Nalog koji koristite za pokretanje simuliranih napada zahteva dozvole globalnog administratora ili administratora bezbednosti i višestruku potvrdu identiteta (MFA). Više informacija o zahtevima simulatora napada potražite u [ovoj temi.](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator)

- Važne stvari koje treba znati o **simulacijama** napada brute i lozinke:

  - Ako ciljni nalog ima omogućen MFA, a lozinka je ispravno pogađana, nalog se neće prikazati kao ugrožen (drugi faktor za potvrdu identiteta će biti nedovršen).

  - Datoteka lozinke ne može biti veća od 10 MB. Koristite jednu lozinku po redu i unesite prazan red (povratak na polje reda) posle poslednje lozinke na listi.

- Važne stvari koje treba znati **o Spear phishingu** prilaže simulacije:

  - Po dizajnu, ne možete da obezbedite prilagođenu vrednost za **URL adresu servera** za prijavljivanje na Phishing.

  - Ako primalac koristi programski dodatak Omogući poruku izveštaja da prijavi poruku kao phishing, možda neće primiti obaveštenja za poruku (zato što je [to](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) simulirani napad).

- Izveštaji: Kada se simulirani napad dovrši, možete da kliknete na dugme Detalji **o napadu** da biste videli izveštaj.

- Detaljna uputstva i nove funkcije u simulatoru napada pogledajte u [temi Simulator napada u operativnom Microsoft 365.](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator)
