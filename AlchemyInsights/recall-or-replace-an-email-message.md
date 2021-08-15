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
ms.openlocfilehash: 45882b49c5c47b3e0e4519e2339e6c68110bc75aebeaeac2d0ccd009bdfa3f7e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "54024400"
---
# <a name="recall-or-replace-an-email-message-in-microsoft-365"></a>Opozovete ili zamenite e-poruku u Microsoft 365

- Možete **opozivati samo poruke koje su poslate osobama iz vaše organizacije.** Na primer, ako je poruka poslata na Gmail adresu, ne možete da je se setite.
- Poruke **poslate sa računara možete da opozvane samo Outlook sa računara.** Ako korisnik pošalje poruku pomoću programa Outlook za Mac ili Outlook na vebu, ne možete da je opozovete.
- Kao administrator zakupaca možete da opozovete poruke u ime korisnika tako što ćete koristiti **PowerShell** (više informacija potražite u: Pretraživanje i brisanje [e-poruka](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization)).
- Poruke iz centra za adminise ne možete da opozvane. Pomerite se nadole do stavke "Potražite i izbrišite e-poruke u organizaciji" da biste dobili više informacija.

**Opoziv ili zamena e-poruke koju ste poslali**

1. U oknu fascikle sa leve strane prozora Outlook odaberite fasciklu Poslate stavke.
2. Otvorite poruku koju želite da opozozete. Morate da kliknete dvaput da biste otvorili poruku. Ako izaberete poruku tako da se ona pojavi u oknu za čitanje, nećete moći da je opozvate.
3. Na kartici Poruka izaberite stavku **Radnje**  >  **Opozvane ovu poruku.**
4. Odaberite **Izbriši nepročitane kopije ove** poruke ili Izbriši nepročitane **kopije** i zameni ih novom porukom, a zatim kliknite na dugme **U redu.**
5. Ako šaljete zamennu poruku, sastavite poruku i izaberite stavku **Pošalji**.
6. Uspeh ili neuspeh opoziva poruke zavisi od postavki primalaca u programu Outlook.

Više informacija, uključujući i to kako da proverite opoziv, potražite u temi Opoziv [ili zamena e-poruke koju ste poslali.](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0)

***Da biste pretražili i*** izbrisali e-poruke u organizaciji, to je najlakše ako ste globalni admin. Ako niste globalni admini svom nalogu, morate da se dodate u grupu uloga menadžera e-pošte ili u ulogu upravljanja pretragom usaglašenosti. Da biste izbrisali poruke, morate da se pridružite grupi uloga "Upravljanje organizacijom" ili ulozi upravljanja pretragom i brisanjem. Dozvole za ove uloge dodeljene su u centru za & za [usaglašenost bezbednosti.](https://protection.office.com/)

1. [Kreirajte pretragu sadržaja](https://docs.microsoft.com/microsoft-365/compliance/content-search) da biste pronašli poruku za brisanje.
2. [Povezivanje u PowerShell & za usaglašenost.](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell)

Ako koristite MFA (višestruku potvrdu identiteta), pogledajte Povezivanje da Microsoft 365 Centar za & usaglašenost usluge PowerShell pomoću višestruke potvrde [identiteta.](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)
