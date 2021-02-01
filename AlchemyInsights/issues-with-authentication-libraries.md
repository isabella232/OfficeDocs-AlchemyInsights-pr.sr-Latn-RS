---
title: Problemi sa bibliotekama za potvrdu identiteta
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004333"
- "7731"
ms.openlocfilehash: ab4ffbc78a7cadd8acee3c98eaa5f3323da9c7e3
ms.sourcegitcommit: 7e6d89f47eca1babf5aeba4995bceccd990c3963
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 01/28/2021
ms.locfileid: "50063643"
---
# <a name="issues-with-authentication-libraries"></a>Problemi sa bibliotekama za potvrdu identiteta

1. [Biblioteke Microsoft aplikacije za proveru](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) identiteta za identifikaciju navode na klijentske i kompatacije klijenta za Microsoft aplikacije.
2. Microsoft biblioteka autentifikacije (MSAL) podržava nekoliko [tokova autentičnosti](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows) za korišćenje u razlicitim scenarijima aplikacije.
3. Da biste potvrdili identitet i nabavili Tokene, inicijalno ste pokrenuli novu javnu ili poverljivu aplikaciju klijenta u kodu. Možete da konfigurišete nekoliko opcija za konfigurisanje kada pokrenete aplikaciju klijenta u Microsoft biblioteci autentifikacije (MSAL). Da biste saznali više, pogledajte odeljak [opcije konfiguracije aplikacija](https://docs.microsoft.com/azure/active-directory/develop/msal-client-application-configuration).

**Kraj podrške za Azure Active Directory potvrda identiteta biblioteke (ADALE) i Azure AD Graph Graf (AAD Graph)**

**Počevši od 30 juna, 2020**, više nećemo dodavati nove funkcije na adale i AZURE AD Graf. Nastavićemo da pružamo tehničku podršku i bezbednosne ispravke, ali više nećemo pružati ispravke funkcija.

**Počevši od 30 juna, 2022**, završićemo podršku za Adale i AZURE AD Graf i neće više pružiti tehničku podršku ili bezbednosne ispravke.

Aplikacije koje koriste ADAL na postojećim verzijama OS nastaviće da funkcionišu posle ovog vremena, ali neće *dobiti tehničku podršku ili bezbednosne ispravke*.

Aplikacije koje koriste Azure AD Graph posle ovog vremena možda više neće primati odgovore od krajnje tačke Azure oglasa Graph.

**ADALA migracija**

Preporučujemo ažuriranje na [Microsoft Authentication Library (MSAL) ](https://docs.microsoft.com/azure/active-directory/develop/v2-overview)koja ima najnovije funkcije i bezbednosne ispravke.

Ako koristite Microsoft aplikacije, znajte da je Microsoft u procesu migriranja svojih aplikacija u MSAL pomoću krajnjeg roka za podršku, kako bi obezbedio korist od trenutne bezbednosti MSALA i poboljšanja funkcija.

Za više informacija pogledajte članak:

1. [Pročitajte najčešća pitanja za ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [Saznajte više o tome kako da migrirate aplikacije na osnovu platforme](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. Ako vam je potrebna pomoć da biste razumeli koje aplikacije koriste ADALE, preporučujemo da pregledate sve izvorne kodove za aplikacije i ako je to primenljivo, da pristupite bilo kom dobavljaču ili dobavljačima aplikacija. Microsoft podrška vam takođe može pružiti listu svih aplikacija koje nisu Microsoft ADAL u vašem zakupcu.

**AAD Graph migracija**

Za aplikacije koje koriste Azure AD Graph, potražite uputstvo za [migraciju AZURE AD Graph grafika u Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview).

1. [Naša kontrolna lista za migraciju pruža taиku na početku.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)
2. Vaš portal za registraciju aplikacija Azure prikazuje koje aplikacije koriste AAD Graph. Preporučujemo vam da pregledate sav izvorni kod aplikacija i, ako je primenljivo, kontaktirate bilo koje ISV-ove ili dobavljače aplikacija. Microsoft podrška vam takođe može pružiti listu svih podrške za AAD Graph u zakupcu.
3. Da bi aplikacija pristupala podacima u programu Microsoft Graph, korisnik ili administrator mora da joj dodeli ispravne dozvole putem procesa pristanka. [Referenca sa Microsoft Graph dozvolama](https://docs.microsoft.com/graph/permissions-reference) navodi dozvole povezane sa svakim glavnim skupom Microsoft Graph API. On takođe pruža uputstva o tome kako da koristite dozvole.
