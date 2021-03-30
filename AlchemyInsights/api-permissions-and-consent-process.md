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
ms.openlocfilehash: 23fed786e7b33adf0b6c76fc71a7e69f2cfcceb7
ms.sourcegitcommit: e5f261f95ffc6074cce89e62ef8c4e9fd519d3ee
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 03/26/2021
ms.locfileid: "51405439"
---
# <a name="api-permissions-and-consent-process"></a>API dozvole i proces pristanka

Da bi aplikacija pristupili podacima u programu Microsoft Graph, korisnik ili administrator moraju da im dodele odgovarajuće dozvole putem procesa pristanka. [Microsoft Graph reference za dozvole](https://docs.microsoft.com/graph/permissions-reference) navodi dozvole povezane sa svakim glavnim skupom Microsoft Graph AČI-ja. Takođe pruža uputstva o tome kako da koristite dozvole.

**Podešavanje ili ažuriranje principala usluge**

- [Kreirajte serviceprincipal](https://docs.microsoft.com/graph/api/serviceprincipal-post-serviceprincipals) – Ovaj članak vam pokazuje kako da kreirate novi servicePrincipal objekat.
- Na portalu kreirajte principal [usluge & Azure AD](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) – Ovaj članak vam pokazuje kako da kreirate novu Azure Active Directory (Azure AD) aplikaciju i principal usluge koja može da se koristi sa kontrolom pristupa zasnovanom na ulozi.
- Aplikacije & glavnice usluga u [usluzi Azure AD](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) – Ovaj članak opisuje registraciju, objekte aplikacije i principale usluga u usluzi Azure Active Directory: šta su, kako se koriste i kako su međusobno povezani.

**Dodajte ili ažurirajte registraciju aplikacije i pružite saglasnost za administarcionu aplikaciju**

- [Kreiranje registracije aplikacije](https://docs.microsoft.com/graph/api/application-post-applications) – Ovaj članak vam pokazuje kako da kreirate novi objekat aplikacije.
- [Ažuriranje registracije aplikacije – API dozvole](https://docs.microsoft.com/graph/api/application-update) – Ovaj članak vam pokazuje kako da ažurirate svojstva objekta aplikacije.
- [Pružite saglasnost](https://docs.microsoft.com/graph/security-authorization#grant-permissions-to-an-application) za adminitre – Za saglasnost i saglasnost u principu, zahtevamo da se saglasnost izričito izričito dodeli.
- [RBAC (beta)](https://docs.microsoft.com/graph/api/resources/rbacapplicationmultiple) – kontejner za upravljanje ulogom za definicije uloga i dodele uloga za Microsoft 365 RBAC dobavljače koji podržavaju više principala i višestruke prognoze u dodeli jedne uloge. Ovaj tip resursa se razlikuje od *rbacApplication* resursa. Microsoft Intune je primer takvog RBAC dobavljača. Dodela uloge u funkciji Intune može da ima niz principala i niz grupa škodova. **To je u beta progamu, što znači da je i dalje u razvoju i ne preporučuje se za upotrebu u proizvodnji.**
