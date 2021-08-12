---
title: API dozvole i proces pristanka
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004345"
- "9200"
ms.openlocfilehash: 078f5798533dfbbf97858f305729f103663644fee3590cdcc877233041adae81
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "53932075"
---
# <a name="api-permissions-and-consent-process"></a>API dozvole i proces pristanka

Da bi vaša aplikacija pristupala podacima u sistemu Microsoft Graph, korisnik ili administrator moraju da im dodele odgovarajuće dozvole putem procesa pristanka. [Microsoft Graph navodi dozvole povezane](https://docs.microsoft.com/graph/permissions-reference) sa svakim glavnim skupom Microsoft Graph APU-ja. Takođe pruža uputstva o tome kako da koristite dozvole.

**Podešavanje ili ažuriranje principala usluge**

- [Kreirajte serviceprincipal](https://docs.microsoft.com/graph/api/serviceprincipal-post-serviceprincipals) – Ovaj članak vam pokazuje kako da kreirate novi servicePrincipal objekat.
- [Kreirajte Azure AD](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) aplikaciju & principal usluge na portalu – Ovaj članak vam pokazuje kako da napravite novu Azure Active Directory (Azure AD) aplikaciju i principal usluge koja može da se koristi sa kontrolom pristupa zasnovanom na ulozi.
- Aplikacije & glavnice usluga u [usluzi Azure AD](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) – Ovaj članak opisuje registraciju, objekte aplikacije i principale usluga u Azure Active Directory: šta su, kako se koriste i kako su međusobno povezani.

**Dodajte ili ažurirajte registraciju aplikacije i pružite saglasnost za administarcionu aplikaciju**

- [Kreiranje registracije aplikacije](https://docs.microsoft.com/graph/api/application-post-applications) – Ovaj članak vam pokazuje kako da kreirate novi objekat aplikacije.
- [Ažuriranje registracije aplikacije – API dozvole](https://docs.microsoft.com/graph/api/application-update) – Ovaj članak vam pokazuje kako da ažurirate svojstva objekta aplikacije.
- [Pružite saglasnost](https://docs.microsoft.com/graph/security-authorization#grant-permissions-to-an-application) za adminitre – Za saglasnost i saglasnost u principu, zahtevamo da se saglasnost izričito izričito dodeli.
- [RBAC (beta)](https://docs.microsoft.com/graph/api/resources/rbacapplicationmultiple) – kontejner za upravljanje ulogom za definicije uloga i dodele uloga za dobavljače Microsoft 365 RBAC koji podržavaju više principala i višestruke prognoze u dodeli jedne uloge. Ovaj tip resursa se razlikuje od *rbacApplication* resursa. Microsoft Intune je primer takvog dobavljača RBAC. Dodela uloge u funkciji Intune može da ima niz principala i niz grupa škodova. **To je u beta progamu, što znači da je i dalje u razvoju i ne preporučuje se za upotrebu u proizvodnji.**
