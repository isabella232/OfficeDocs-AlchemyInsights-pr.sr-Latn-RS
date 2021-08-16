---
title: Problemi sa bibliotekama potvrde identiteta
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
ms.openlocfilehash: 39336fa8840a28befcad449d0afa59c1df5c6bef5988cb197916a03aa2aa66c9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028018"
---
# <a name="issues-with-authentication-libraries"></a>Problemi sa bibliotekama potvrde identiteta

1. [Microsoft platforma za identitete biblioteke potvrde identiteta](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) navode biblioteke klijenta i srednjeg softvera podržane i kompatibilne biblioteke klijenta i srednjeg softvera.
2. Microsoft biblioteka za potvrdu identiteta (MSAL) podržava nekoliko tokova potvrde identiteta [za](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows) korišćenje u različitim scenarijima aplikacija.
3. Da biste potvrdili identitet i preuzeli tokene, možete da inicijalizujete novu javnu ili poverljivu klijentski aplikaciju u kodu. Možete da podesite nekoliko opcija konfiguracije prilikom pokretanja klijentske aplikacije u Microsoft biblioteci za potvrdu identiteta (MSAL). Da biste saznali više, pogledajte opcije [konfiguracije aplikacije.](https://docs.microsoft.com/azure/active-directory/develop/msal-client-application-configuration)

**Kraj podrške za Azure Active Directory biblioteke potvrde identiteta (ADAL) i Azure AD Graph API (AAD Graph)**

**Počev od 30. juna 2020.** više nećemo dodavati nove funkcije u ADAL i Azure AD Graph. Nastavićemo da pružamo tehničku podršku i bezbednosne ispravke, ali više nećemo pružati ispravke funkcija.

**Počev od 30. juna 2022,** završićemo podršku za ADAL i Azure AD Graph i više nećemo pružati tehničku podršku ili bezbednosne ispravke.

Aplikacije koje koriste ADAL u postojećim verzijama operativnog sistema nastaviće da rade posle tog vremena, ali neće dobiti tehničku podršku *ili bezbednosne ispravke.*

Aplikacije koje koriste Azure AD Graph nakon tog vremena, možda više neće primati odgovore iz Azure AD Graph krajnje tačke.

**ADAL migracija**

Preporučujemo ažuriranje na [Microsoft Authentication Library (MSAL) ](https://docs.microsoft.com/azure/active-directory/develop/v2-overview)koja ima najnovije funkcije i bezbednosne ispravke.

Ako koristite Microsoft aplikacije, znajte da je Microsoft u procesu migriranje aplikacija u MSAL do kraja roka podrške, obezbeđujući da će imati koristi od tekućih poboljšanja bezbednosti i funkcija MSAL.

Za više informacija pogledajte:

1. [Pročitajte najčešća pitanja za ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [Saznajte više o tome kako da migrirate aplikacije na osnovu platforme](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. Ako vam je potrebna pomoć da razumete koje aplikacije koriste ADAL, preporučujemo da pregledate izvorni kôd svih aplikacija i, ako je primenljivo, vašoj dobavljačima ISV usluga ili aplikacija. Microsoft podrška vam takođe može pružiti listu svih aplikacija koje nisu Microsoft ADAL u vašem zakupcu.

**AAD Graph migracija**

Za aplikacije koje koriste Azure AD Graph, pratite uputstva da biste migrirali [Azure AD Graph aplikacije](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview)u Microsoft Graph.

1. [Naša lista za proveru migracije pruža mesto za početak.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)
2. Vaš portal za registraciju aplikacija Azure prikazuje koje aplikacije koriste AAD Graph. Preporučujemo vam da pregledate sav izvorni kod aplikacija i, ako je primenljivo, kontaktirate bilo koje ISV-ove ili dobavljače aplikacija. Microsoft podrška vam takođe može pružiti listu svih AAD Graph koji se koristi u vašem zakučaru.
3. Da bi vaša aplikacija pristupala podacima u sistemu Microsoft Graph, korisnik ili administrator moraju da im dodele odgovarajuće dozvole putem procesa pristanka. Microsoft [Graph za dozvole](https://docs.microsoft.com/graph/permissions-reference) navodi dozvole povezane sa svakim glavnim skupom Microsoft Graph APU-ja. Takođe pruža uputstva o tome kako da koristite dozvole.
