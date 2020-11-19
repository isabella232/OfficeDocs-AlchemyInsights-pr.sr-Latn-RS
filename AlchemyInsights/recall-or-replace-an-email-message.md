---
title: Opoziv ili zamena e-poruke
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1860"
- "9000260"
ms.assetid: ''
ms.openlocfilehash: 05016213a1387c5290cb5899359f1f10b5a413c0
ms.sourcegitcommit: 4e0ae808ee2a586339b396320e3edb8ba066a91a
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 11/19/2020
ms.locfileid: "49353520"
---
# <a name="recall-or-replace-an-email-message-in-microsoft-365"></a>Opoziv ili zamena e-poruke u usluzi Microsoft 365

- Možete da **opozovete poruke koje se šalju osobama u vašoj organizaciji**. Na primer, ako je poruka poslata na gmail adresu, ne možete da je opozovete.
- Možete **samo da opozovete poruke poslate iz programa Outlook za PC**. Ako korisnik pošalje poruku pomoću programa Outlook za Mac ili Outlook na vebu, ne možete da ga opozovete.
- Kao administrator zakupca, možete da **opozovete poruke u ime korisnika pomoću programa PowerShell** (više informacija potražite u članku: [pretraživanje i brisanje e-poruka](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization)).
- Ne možete da opozovete poruke iz centra administracije. Pomerajte se nadole do stavke "Pretraga i brisanje e-poruka u organizaciji" za više informacija.

**Opoziv ili zamena e-poruke koju ste poslali**

1. U oknu sa fasciklama na levoj strani prozora programa Outlook Odaberite fasciklu poslate stavke.
2. Otvorite poruku koju želite da opozovete. Morate da kliknete dvaput da biste otvorili poruku. Izbor poruke tako da se pojavljuje u oknu za čitanje neće vam omogućiti da opozovete poruku.
3. Na kartici poruka izaberite **stavke Radnje**  >  **Opozovi ovu poruku**.
4. Odaberite stavku **Izbriši nepročitane kopije ove poruke** ili **Izbriši nepročitane kopije i zameni je novom porukom**, a zatim kliknite na **dugme u redu**.
5. Ako šaljete poruku za zamenu, sastavite poruku, a zatim izaberite **Pošalji**.
6. Uspeh ili otkazivanje opoziva poruke zavisi od postavki primalaca u programu Outlook.

Više informacija o tome kako da potvrdite opoziv potražite u članku [opoziv ili zamena e-poruke koju ste poslali](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).

**_Da biste pretražili i izbrisali e-poruke u organizaciji_**, to je najlakše ako ste globalni administrator. Ako niste globalni administrator, nalog mora da se doda u grupu uloga menadžera eDiscovery ili na ulogu upravljanja usaglašenosti. Da biste izbrisali poruke, moraćete da se pridružite grupi uloga za upravljanje organizacijom ili svojoj ulozi za pretraživanje i čišćenje. Dozvole za ove uloge se dodeljuju u [centru za bezbednost & bezbednosti](https://protection.office.com/).

1. [Kreirajte pretragu sadržaja](https://docs.microsoft.com/microsoft-365/compliance/content-search) da biste pronašli poruku za brisanje.
2. [Povezivanje sa bezbednosnim & PowerShell Center usaglašenosti](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell).

Ako koristite MFA (multifaktor verifikacije identiteta), pogledajte članak [Povezivanje sa uslugom Microsoft 365 Security & centar za usaglašenost sa PowerShell pomoću multifaktor potvrde identiteta](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell).
