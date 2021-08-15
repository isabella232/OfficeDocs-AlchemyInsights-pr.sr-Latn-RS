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
ms.openlocfilehash: 7058b6419e52fce94f3359d0bd8e1d67c5aa5ef6743abf4ed39f45bad49e1d07
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "54025624"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a>Treba da označite domen ili pošiljaoca e-pošte kao bezbedne?

- Ne preporučuje se **korišćenje lista** bezbednih pošiljalaca jer otvara vašu organizaciju za napade kao što su upućivanje od phish i phishova.
- Međutim, ako postoji poslovni zahtev, preporučujemo **da** za to koristite **[Flow Pravila za](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** poštu. Naša uputstva obezbeđuju da pošiljalac potvrde identiteta (potvrđuje da domen koji šaljete nije potvrđen) nije potvrđen. Napomena: Ne preporučujemo da upravljate pozitivnim informacijama o netačnim pošiljaocima pomoću lista bezbednih pošiljalaca jer izuzeci za filtriranje bez-pošte mogu da otvore organizaciju za bezbednosne **napade.** Ako korisnici neispravno primaju poruke koje su pogrešno označene kao bezvredna ili neželjena e-pošta, prijavite poruke **[i datoteke korporaciji Microsoft](https://protection.office.com/reportsubmission)**.
- Sef Treba izbegavati pošiljaoce na Outlook, listi dozvoljenih pošiljalaca ili listi dozvoljenih domena u smernicama za borbu protiv bezverne e-poruke zato što pošiljaoci zaobiđu svu bez-pošiljku, phish zaštitu i phish zaštitu i potvrdu identiteta pošiljaoca (SPF, DKIM, DMARC).  Ovaj metod je najbolje koristiti samo za privremeno testiranje.
- Provera valjanosti da određena procena premošćavanja e-pošte može da se obavi tako što će proveriti zaglavlje poruke "X-Forefront-Antispam-Report" (SFV:SFE, SFV:SKA, SFV:SKN) u zaglavljima poruka protiv **[spam](https://docs.microsoft.com/microsoft-365/security/office-365-security/anti-spam-message-headers)** pošte.
- Pošto Microsoft podrazumevano želi da našim klijentima obezbedi uslugu [,](https://docs.microsoft.com/microsoft-365/security/office-365-security/secure-by-default#exceptions)neke zamene zakupca se ne primenjuju na malver i phishing velike pouzdanosti. Ove zamene uključuju: o Liste dozvoljenih pošiljalaca ili liste dozvoljenih domena (smernice za borbu protiv spam pošte) o Outlook Sef Pošiljaoci O IP liste dozvoljenih (filtriranje veze) 
- Jedina zamena koja omogućava phishing poruci velike pouzdanosti da zaobilazi filtriranje jeste Exchange pravila za tok pošte (poznata i kao pravila prenosa). Da biste koristili pravila za protok pošte da biste zaobišli filtriranje, pogledajte korišćenje pravila za protok pošte za postavljanje nivoa pouzdanosti pošte **[(SCL) u porukama.](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-mail-flow-rules-to-set-the-spam-confidence-level-scl-in-messages)**