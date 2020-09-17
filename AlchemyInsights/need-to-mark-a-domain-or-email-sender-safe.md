---
title: Treba da označite domen ili pošiljalac e-pošte bezbedan?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002921"
- "5673"
ms.openlocfilehash: 0ea089b95ad7de25e77017196fb2db895d4d0178
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 09/15/2020
ms.locfileid: "47803259"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a>Treba da označite domen ili pošiljalac e-pošte bezbedan?

- Korišćenje **Lista bezbednih pošiljalaca se ne preporučuje** jer otvara vašu organizaciju u spam, Fish i lažne napade.
- Međutim, ako postoji uslov za posao, **preporučujemo** da koristite **[pravila toka pošte](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** za ovo. Naše vođstvo osigurava potvrdu identiteta pošiljaoca (Verifikacija slanja domena nije lažnjava). **Napomena**: ne preporučujemo da upravljate lažnim sigurnošću pomoću lista pouzdanih pošiljalaca, jer izuzeci od filtriranja bezvredne pošte mogu da otvore vašu organizaciju bezbednosnim napadima. Ako korisnici primaju poruke koje su pogrešno označene kao bezvredne ili neželjene e-pošte, **[Prijavite poruke i datoteke korporaciji Microsoft](https://protection.office.com/reportsubmission)**.
- Pouzdani pošiljaoci u programu Outlook, dozvoljeni spisak poљiljaocu ili dozvoljenu listu domena u smernicama za borbu protiv bezvredne pošte **treba izbegavati** zato što pošiljaoci zaobilaze sve bezvredne, podve i Phish potvrdu identiteta pošiljaoca (SPF, dkim, dmarc). Ovaj metod se najbolje koristi samo za privremeno testiranje.
