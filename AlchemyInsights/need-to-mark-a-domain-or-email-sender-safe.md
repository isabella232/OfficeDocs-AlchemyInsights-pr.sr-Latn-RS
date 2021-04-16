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
ms.openlocfilehash: a1c4c4d2fadaf75eda9b5b322aca35c32dfee8ea
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 04/15/2021
ms.locfileid: "51792146"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a>Treba da označite domen ili pošiljaoca e-pošte kao bezbedne?

- Ne preporučuje se **korišćenje lista** bezbednih pošiljalaca jer otvara vašu organizaciju za napade kao što su upućivanje od phish i phishova.
- Međutim, ako postoji poslovni zahtev, preporučujemo **da** za to **[koristite pravila](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** za protok pošte. Naša uputstva obezbeđuju da pošiljalac potvrde identiteta (potvrđuje da domen koji šaljete nije potvrđen) nije potvrđen. Napomena: Ne preporučujemo da upravljate pozitivnim informacijama o netačnim pošiljaocima pomoću lista bezbednih pošiljalaca jer izuzeci za filtriranje bez-pošte mogu da otvore organizaciju za bezbednosne **napade.** Ako korisnici neispravno primaju poruke koje su pogrešno označene kao bezvredna ili neželjena e-pošta, prijavite poruke **[i datoteke korporaciji Microsoft](https://protection.office.com/reportsubmission)**.
- Bezbedni pošiljaoci u programu Outlook, listi dozvoljenih  pošiljalaca ili listi dozvoljenih domena u smernicama za borbu protiv bezverne e-poruke trebalo bi izbegavati zato što pošiljaoci zaobiđu svu bezvernu, phish zaštitu i phish zaštitu i potvrdu identiteta pošiljaoca (SPF, DKIM, DMARC). Ovaj metod je najbolje koristiti samo za privremeno testiranje.
