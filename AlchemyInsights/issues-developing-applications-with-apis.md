---
title: Problemi u razvoju aplikacija sa ANIM-ovima
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004343"
- "7755"
ms.openlocfilehash: 1de4e9aa5078507eecdbe53366e446e733029ecb1342f20ca701fa7f95a06fa9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "54013474"
---
# <a name="issues-developing-applications-with-apis"></a>Problemi u razvoju aplikacija sa ANIM-ovima

Da biste počeli da koristite Azure Active Directory Graph API, pogledajte vodič za brzi početak za [Azure AD Graph](https://docs.microsoft.com/azure/active-directory/develop/microsoft-graph-intro) ili prikažite interaktivnu [Azure AD Graph API referentnu](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/api-catalog)dokumentaciju.

**Kraj podrške za Azure Active Directory biblioteke potvrde identiteta (ADAL) i Azure AD Graph API (AAD Graph)**

**Počev od 30. juna 2020.** više nećemo dodavati nove funkcije u ADAL i Azure AD Graph. Nastavićemo da pružamo tehničku podršku i bezbednosne ispravke, ali više nećemo pružati ispravke funkcija.

**Počev od 30. juna 2022,** završićemo podršku za ADAL i Azure AD Graph i više nećemo pružati tehničku podršku ili bezbednosne ispravke.

Aplikacije koje koriste ADAL na postojećim verzijama OS nastaviće da rade i nakon ovog vremena, ali neće dobiti nikakvu tehničku podršku ili bezbednosne ispravke.

Aplikacije koje koriste Azure AD Graph nakon tog vremena, možda više neće primati odgovore iz Azure AD Graph krajnje tačke.

**ADAL migracija**

Preporučujemo ažuriranje na [Microsoft Authentication Library (MSAL) ](https://docs.microsoft.com/azure/active-directory/develop/v2-overview)koja ima najnovije funkcije i bezbednosne ispravke.

Ako koristite Microsoft aplikacije, znajte da microsoft trenutno migrira aplikacije u MSAL do kraja roka podrške, obezbeđujući da će imati koristi od tekućih poboljšanja bezbednosti i funkcija funkcije MSAL.

1. [Pročitajte najčešća pitanja o ADAL- u](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).
1. [Saznajte više o tome kako da migrirate aplikacije na osnovu platforme.](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
1. Ako vam je potrebna pomoć da razumete koje aplikacije koriste ADAL, preporučujemo da pregledate izvorni kôd svih aplikacija i, ako je primenljivo, vašoj dobavljačima ISV usluga ili aplikacija. Microsoft podrška vam takođe može pružiti listu svih aplikacija koje nisu Microsoft ADAL u vašem zakupcu.

**AAD Graph migracija**

Za aplikacije koje koriste Azure AD Graph, pratite uputstva da biste migrirali [Azure AD Graph aplikacije](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview?view=graph-rest-1.0&preserve-view=true)u Microsoft Graph.

1. [Naša lista za migraciju pruža tačku za početak](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
1. Vaš portal za registraciju aplikacija Azure prikazuje koje aplikacije koriste AAD Graph. Preporučujemo vam da pregledate sav izvorni kod aplikacija i, ako je primenljivo, kontaktirate bilo koje ISV-ove ili dobavljače aplikacija. Microsoft podrška vam takođe može pružiti listu svih AAD Graph koji se koristi u vašem zakučaru.
1. Da bi vaša aplikacija pristupala podacima u sistemu Microsoft Graph, korisnik ili administrator moraju da im dodele odgovarajuće dozvole putem procesa pristanka. Microsoft [Graph za dozvole](https://docs.microsoft.com/graph/permissions-reference?context=graph%2Fapi%2Fbeta&view=graph-rest-beta&preserve-view=true) navodi dozvole povezane sa svakim glavnim skupom Microsoft Graph APU-ja. Takođe pruža uputstva o tome kako da koristite dozvole.
