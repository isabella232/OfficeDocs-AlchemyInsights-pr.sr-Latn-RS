---
title: Problemi sa razvojem aplikacija sa Appis
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
ms.openlocfilehash: 26d732819b64efa4fb84da44cc2a279368aa28b0
ms.sourcegitcommit: 605a73b159d30634b064c1b63b0e734ceb3fdec8
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 01/25/2021
ms.locfileid: "49975016"
---
# <a name="issues-developing-applications-with-apis"></a>Problemi sa razvojem aplikacija sa Appis

Da biste počeli da koristite Azure Active Directory Graph API, pogledajte " [AZURE AD Graph grafikon" brzi Start "vodiča](https://docs.microsoft.com/azure/active-directory/develop/microsoft-graph-intro) ili Prikažite [interaktivnu dokumentaciju Azure AD Graph AD Graph](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/api-catalog).

**Kraj podrške za Azure Active Directory potvrda identiteta biblioteke (ADALE) i Azure AD Graph Graf (AAD Graph)**

**Počevši od 30 juna, 2020**, više nećemo dodavati nove funkcije na adale i AZURE AD Graf. Nastavićemo da pružamo tehničku podršku i bezbednosne ispravke, ali više nećemo pružati ispravke funkcija.

**Počevši od 30 juna, 2022**, završićemo podršku za Adale i AZURE AD Graf i neće više pružiti tehničku podršku ili bezbednosne ispravke.

Aplikacije koje koriste ADAL na postojećim verzijama OS nastaviće da funkcionišu posle ovog vremena, ali neće dobiti tehničku podršku ili bezbednosne ispravke.

Aplikacije koje koriste Azure AD Graph posle ovog vremena možda više neće primati odgovore od krajnje tačke Azure oglasa Graph.

**ADALA migracija**

Preporučujemo da ažurirate u [Microsoft biblioteci autentifikacije (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), koja ima najnovije funkcije i bezbednosne ispravke.

Ako koristite Microsoft aplikacije, znajte da je Microsoft u procesu migriranja svojih aplikacija u MSAL pomoću krajnjeg roka za podršku, kada se osigura da će imati koristi od MSALOVE trenutne bezbednosti i poboljšanja funkcija.

1. [Pročitajte Adala najčešća pitanja](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).
1. [Saznajte kako da migrirate aplikacije na osnovu osnove po platformoji](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).
1. Ako vam je potrebna pomoć da biste razumeli koje aplikacije koriste ADALE, preporučujemo da pregledate sve izvorne kodove za aplikacije i ako je to primenljivo, da pristupite bilo kom dobavljaču ili dobavljačima aplikacija. Microsoft podrška vam takođe može pružiti listu svih aplikacija koje ne podržavaju Microsoft u vašem zakupcu.

**AAD Graph migracija**

Za aplikacije koje koriste Azure AD Graph, potražite uputstvo za migraciju [AZURE AD Graph grafika u Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview?view=graph-rest-1.0&preserve-view=true).

1. [Naša kontrolna lista za migraciju pruža taиku na početku](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
1. Vaš Azure registracioni portal pokazuje koje aplikacije koriste AAD Graph. Preporučujemo da pregledate sve izvorne kodove za aplikacije i ako je to primenljivo, da pristupite bilo kom dobavljaču ili dobavljačima aplikacija. Microsoft podrška vam takođe može pružiti listu svih podrške za AAD Graph u zakupcu.
1. Da bi aplikacija pristupala podacima u programu Microsoft Graph, korisnik ili administrator mora da joj dodeli ispravne dozvole putem procesa pristanka. [Referenca sa Microsoft Graph dozvolama](https://docs.microsoft.com/graph/permissions-reference?context=graph%2Fapi%2Fbeta&view=graph-rest-beta&preserve-view=true) navodi dozvole povezane sa svakim glavnim skupom Microsoft Graph API. On takođe pruža uputstva o tome kako da koristite dozvole.
