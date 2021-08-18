---
title: Treba da označite domen ili pošiljaoca e-pošte kao bezbedne?
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002921"
- "5673"
ms.openlocfilehash: afc865a7b91036bd2d982e21dce059a87e109e3e
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/13/2021
ms.locfileid: "58319962"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a>Treba da označite domen ili pošiljaoca e-pošte kao bezbedne?

- Ne preporučuje se **korišćenje lista** bezbednih pošiljalaca jer otvara vašu organizaciju za napade na poruke, phish i napade koji se tiču phishova.
- Međutim, ako postoji poslovni zahtev, preporučujemo **da** za **[ovo koristite Flow Pravila za](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** poštu. Naša uputstva obezbeđuju da pošiljalac potvrde identiteta (potvrđuje da domen koji šaljete nije potvrđen) nije potvrđen. 
    Napomena: Ne preporučujemo da upravljate pozitivnim informacijama o netačnim pošiljaocima pomoću lista bezbednih pošiljalaca jer izuzeci za filtriranje bez-pošte mogu da otvore organizaciju za bezbednosne **napade.** Ako korisnici neispravno primaju poruke koje su pogrešno označene kao bezvredna ili neželjena e-pošta, prijavite poruke **[i datoteke korporaciji Microsoft.](https://protection.office.com/reportsubmission)**
- Sef Pošiljaoci na Outlook, listi dozvoljenih pošiljalaca ili  listi dozvoljenih domena u smernicama za borbu protiv bezverne e-poruke trebalo bi izbegavati zato što pošiljaoci zaobiđu svu bezvernu, phish zaštitu i phish zaštitu i potvrdu identiteta pošiljaoca (SPF, DKIM, DMARC). Ovaj metod je najbolje koristiti samo za privremeno testiranje.
- Provera valjanosti da određena procena premošćavanja e-pošte može da se obavi tako što će proveriti zaglavlje poruke "X-Forefront-Antispam-Report" (SFV:SFE, SFV:SKA, SFV:SKN) u zaglavljima poruka protiv **[spam](https://docs.microsoft.com/microsoft-365/security/office-365-security/anti-spam-message-headers)** pošte.
- Pošto Microsoft podrazumevano želi da našim klijentima obezbedi uslugu [,](https://docs.microsoft.com/microsoft-365/security/office-365-security/secure-by-default#exceptions)neke zamene zakupca se ne primenjuju na malver i phishing velike pouzdanosti. Te zamene uključuju: o Liste dozvoljenih pošiljalaca ili liste dozvoljenih domena (smernice za borbu protiv spam pošte) o Outlook Sef Pošiljaoci sa IP liste dozvoljenih IP adresa (filtriranje veze) 
- Jedina zamena koja omogućava phishing poruci velike pouzdanosti da zaobilazi filtriranje jeste Exchange pravila za tok pošte (poznata i kao pravila prenosa). Da biste koristili pravila za protok pošte da biste zaobišli filtriranje, pogledajte korišćenje pravila za protok pošte za postavljanje nivoa pouzdanosti pošte **[(SCL) u porukama.](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-mail-flow-rules-to-set-the-spam-confidence-level-scl-in-messages)**