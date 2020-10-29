---
title: 2681 simulator napada u programu Microsoft 365
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
ms.openlocfilehash: 7b48abea3400e3565f2ba33c97e24e5b9923eb3b
ms.sourcegitcommit: 4caf5e6c2fee2903ccaf92cfc9006eb580faa7ba
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 10/29/2020
ms.locfileid: "48801565"
---
# <a name="attack-simulator-in-microsoft-365"></a>Simulator napada u programu Microsoft 365

- Nedostaje vam simulator za napad? Simulator napada zahteva **Microsoft Defender za Office 365 plan 2 (ATP plan 2)** ili **Office 365 Enterprise E5** . Simulator napada **nije** uključen u Microsoft Defender za Office 365 plan 1 (ATP plan 1), Office 365 Enterprise E3 ili bilo koje Microsoft 365 aplikacije za pretplatu.

- Nalog koji koristite za pokretanje simuliranih napada zahteva opšte dozvole globalnog administratora ili administratora bezbednosti i potvrdu identiteta sa više faktora (MFA). Više informacija o zahtevima za simulator napada potražite u [ovom članku](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).

- Važne stvari koje treba znati **o** simulacijama za napad

  - Ako je omogućeno MFA za ciljni nalog i ako je lozinka ispravno pogodila, nalog se neće prikazati kao kompromitovan (drugi faktor potvrde identiteta će biti nepotpun).

  - Datoteka lozinki ne može biti veća od 10 MB. Koristite jednu lozinku po redu i dodajte praznu liniju (povratni tip) posle poslednje lozinke na listi.

- Važne stvari koje treba znati o **phishing** Prilaganje Priloži:

  - Po dizajnu, ne možete da obezbedite prilagođenu vrednost za **URL adresu za phishing server za prijavljivanje** .

  - Ako primalac koristi [programski dodatak "Omogućavanje poruke izveštaja](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) " da bi izvestio o grešci kao phishing, možda nećete primati obaveštenja (jer je ovo simulirani napad).

- Izveštaji: kada se završi simulirani napad, možete da kliknete na dugme **Detalji napada** da biste videli izveštaj.

- Detaljna uputstva i nove funkcije u simulatoru za napad potražite [u članku napad simulatora u programu Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).
