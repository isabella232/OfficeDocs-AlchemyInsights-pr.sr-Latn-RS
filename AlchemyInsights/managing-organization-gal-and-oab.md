---
title: Upravljanje globalnim spiskom adresa organizacije i vanmrežnim adresarom
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
- "9002895"
- "5550"
ms.openlocfilehash: c5b73e2dae4d2b98b6af05e147f93a493bac5a88cfcb9ea67c979264aba34ceb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "54042176"
---
# <a name="managing-organization-global-address-list-gal-and-offline-address-book-oab"></a>Upravljanje globalnim spiskom adresa (GAL) organizacije i vanmrežnim adresarom (OAB)

Globalni spisak adresa (GAL) jeste lista objekata omogućenih za poštu (bilo koji tip primaoca koji može da prima e-poštu) u organizaciji. Jedan GAL se automatski kreira u svakoj organizaciji. Dodatni GAL možete da kreirate da biste razdvojili korisnike po organizaciji ili lokaciji, ali jedan korisnik može da vidi i koristi samo jedan GAL odjednom.

Neki klijenti e-pošte, kao što je Outlook za Windows, preuzimaju GAL za vanmrežno korišćenje. Ovo je poznato kao vanmrežni adresar (OAB). U sistemu Exchange online, OAB se ažurira samo jednom na svakih 8 časova i onda klijent mora da ga preuzme da bi ažurirao lokalnu OAB kopiju. Svaka promena primaoca prvo mora biti vidljiva u GAL-u, da bi se kasnije mogla pronaći u OAB-u.

Evo nekih najčešće korišćenih GAL i OAB procedura:

- Iz različitih razloga, možda ćete želeti da neki objekti budu sakriveni od GAL-a. Pogledajte odeljak [Sakrivanje primaoca sa spiska adresa](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#hide-recipients-from-address-lists).
- Ako je potrebno da određenim grupama korisnika date prilagođene prikaze na GAL organizacije, pročitajte članak [Smernice za adresare u sistemu Exchange Online](https://docs.microsoft.com/exchange/address-books/address-book-policies/address-book-policies).
- [Kreirajte globalni spisak adresa u sistemu Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/create-global-address-list) i saznajte kako da radite sa GAL, pročitajte članak [Lista adresa u sistemu Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/address-lists). Imajte u vidu da ako kreirate nove GAL, možda ćete želeti da kreirate i novi OAB. Pogledajte [Procedure za](https://docs.microsoft.com/exchange/address-books/offline-address-books/offline-address-book-procedures)operacije vanmrežnog adresara.
