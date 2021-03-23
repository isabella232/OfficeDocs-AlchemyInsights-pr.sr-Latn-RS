---
title: Rad sa bibliotekama za potvrdu identiteta
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9775"
- "9004342"
ms.openlocfilehash: f9f54ed2bfc5841df66d3e714112b9307455c182
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036870"
---
# <a name="working-with-authentication-libraries"></a>Rad sa bibliotekama za potvrdu identiteta

Da biste rešili problem sa Microsoft bibliotekom identiteta (MSAL), obavite sledeće preporučene korake:

1. **Rad sa uslugom MSAL**: [bibliotekama za potvrdu identiteta Microsoft platforme](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) – ovaj članak prikazuje podršku za Microsoft biblioteku za Microsoft potvrdu identiteta za nekoliko tipova aplikacija. On uključuje veze ka izvornom kodu biblioteke; Gde da nabavite paket za projekat aplikacije? i da li biblioteka podržava korisničko prijavljivanje (potvrda identiteta), pristup zaštićenom vebu Appis (autorizaciju) ili oba.

2. **Rešavanje problema sa autentifikacijom**: msal podržava nekoliko tokova autentičnosti za korišćenje u razlicitim scenarijima aplikacije. U zavisnosti od toga kako se gradi klijentska aplikacija, MSAL može da koristi neki od tokova potvrde identiteta koje podržava Microsoft Platform identiteta. Ovi tokovi mogu da proizvedu nekoliko tipova pozivnih brojeva i kodova za autorizaciju i zahtevaju razne simbole da bi radili.

3. **Access tokena**: [microsoftens Platform za identifikaciju identiteta](https://docs.microsoft.com/azure/active-directory/develop/access-tokens) – Saznajte kako API može da proveri valjanost i koristi zahteve unutar simbola za pristup. Sva dokumentacija u ovom članku, osim gde je navedeno, odnosi se samo na Tokene koji su izdati za APIs koje ste registrovali. Ne odnosi se na oznake koje su izdate za usluge koje posjeduje Microsoft-not, niti se ovi Tokeni mogu koristiti za validaciju načina na koji Microsoft platforma za identifikaciju izdaje tokena za API koji kreirate.

**Kraj podrške za Azure Active Directory potvrda verodostojnosti (ADALE)**

- **Počevši od 30 juna, 2020,** više nećemo dodavati nove funkcije na adale i AZURE AD Graf. Nastavićemo da pružamo tehničku podršku i bezbednosne ispravke, ali više nećemo pružati ispravke funkcija.
- **Počevši od 30 juna, 2022,** Završićemo podršku za Adale i AZURE AD Graf i neće više pružiti tehničku podršku ili bezbednosne ispravke.
- Aplikacije koje koriste ADAL na postojećim verzijama OS nastaviće da funkcionišu posle ovog vremena, ali neće *dobiti tehničku podršku ili bezbednosne ispravke*.
- Aplikacije koje koriste Azure AD Graph posle ovog vremena možda više neće primati odgovore od krajnje tačke Azure oglasa Graph.

**ADALA migracija**

- Preporučujemo da ažurirate MSAL, koji ima najnovije funkcije i bezbednosne ispravke.
- Ako koristite Microsoft aplikacije, znajte da je Microsoft u procesu migriranja svojih aplikacija u MSAL pomoću krajnjeg roka za podršku, kada se osigura da će imati koristi od MSALOVE trenutne bezbednosti i poboljšanja funkcija.

1. [Pročitajte Adala najčešća pitanja](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).
2. [Saznajte kako da migrirate aplikacije na osnovu osnove po platformoji](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#migration-guidance).
3. Ako nakon čitanja vodiča za platformu aplikacije imate dodatna pitanja, možete da knjižite na [lokaciji Microsoft Q&](https://docs.microsoft.com/answers/topics/azure-ad-adal-deprecation.html) sa oznakom [azuri-AD-dprecation] ili da otvorite problem u programu GitHub biblioteke. Pogledajte odeljak [jezici i okviri](https://docs.microsoft.com/azure/active-directory/develop/msal-overview#languages-and-frameworks) **prikaza teksta za veze sa** potvrdom svake biblioteke.
4. **Ako vam je potrebna pomoć da biste razumeli koje aplikacije koriste adno**, preporučujemo vam da pregledate sve izvorne kodove za aplikacije. Ako je to primenljivo, pristupite bilo kom nezavisnom dobavljaču usluga (ISVs) ili dobavljačima aplikacija. Microsoft podrška vam takođe može pružiti listu svih aplikacija koje nisu Microsoft ADAL u vašem zakupcu.







