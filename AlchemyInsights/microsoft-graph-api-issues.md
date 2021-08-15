---
title: Microsoft Graph API problemi
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
- "9004345"
- "7759"
ms.openlocfilehash: 9df021211c8a65997889d9303dbf28a27104cfa95841d4cb810427c652ba0784
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "53975907"
---
# <a name="microsoft-graph-api-issues"></a>Microsoft Graph API problemi

Ova tema može da se primeni i na projektante koji još uvek koriste Azure AD Graph API. Međutim, preporučuje  se da koristite Microsoft Graph za sve scenarije direktorijuma, identiteta i upravljanja pristupom.

**Problemi sa potvrdom identiteta ili autorizacije**

- Ako aplikacija ne može da pribavi **tokene** za pozivanje aplikacije Microsoft Graph, izabrati problem sa dobijanjem **tokena** za pristup (potvrda identiteta) microsoft Graph kategoriji da biste dobili specifičnije pomoć i podršku za ovu temu.
- Ako aplikacija dobija **401 ili 403** greške u autorizovanju prilikom pozivanja korporacije Microsoft Graph, izabrati kategoriju Dobijanje pristupa je odbijen **(Autorizacija)** Microsoft Graph API da biste dobili određeniju pomoć i podršku za ovu temu.

**Želim da koristim Microsoft Graph, ali nisam siguran odakle da počnem**

- [Pregled usluge Microsoft Graph](https://docs.microsoft.com/graph/overview)
- [Pregled upravljanja identitetom i pristupom u programu Microsoft Graph](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [Početak izgradnje Microsoft Graph aplikacija](https://docs.microsoft.com/graph/)
- **Microsoft Graph Explorer** – testiranje Microsoft Graph APIT-ja u zakupca ili demo zakupca

**Želim da koristim Microsoft Graph, ali da li podržava v1.0 AD-je direktorijuma koji su mi potrebni?**

Microsoft Graph je preporučeni API za direktorijum, identitet i upravljanje pristupom. Međutim, postoji još nekoliko razlika između onoga što je moguće u Azure AD Graph i Microsoft Graph. Pregledajte sledeće članke koji ističu najažuarnije razlike da biste pomogli pri izboru:

- [Razlike u tipu resursa između usluge Azure AD Graph i Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [Razlike u svojstvima između usluge Azure AD Graph i Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [Razlike u metodima između Azure AD i Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

**API koji pozivam ne funkcioniše – gde mogu da uradim više testiranja?**

**Microsoft Graph Explorer** – testirajte Microsoft Graph ABE-je u zakupca ili demo  verziji zakupca, a pogledajte i uzorke upita u programu Microsoft Graph Explorer.

**Moja aplikacija je suviše spora i reaguje. Koja poboljšanja mogu da napravim?**

U zavisnosti od scenarija, postoji mnoštvo opcija koje su vam na raspolaganju kako biste aplikaciju načinili performativnijim, a u nekim slučajevima manje ćete biti skloni da ih usluga remeti (kada upućujete previše poziva).

- [Najbolje Graph Microsoft naloga](https://docs.microsoft.com/graph/best-practices-concept)
- [Zahtevi za grupisanje](https://docs.microsoft.com/graph/json-batching)
- [Praćenje promena putem delta upita](https://docs.microsoft.com/graph/delta-query-overview)
- [Dobijanje obaveštenih o promenama putem vebhook-a](https://docs.microsoft.com/graph/webhooks)
- [Uputstvo za oslanjanje](https://docs.microsoft.com/graph/throttling)

**Gde mogu da pronađem više informacija o greškama i poznatim problemima?**

- [Informacije Graph o grešci korporacije Microsoft](https://docs.microsoft.com/graph/errors)
- [Poznati problemi sa Microsoft Graph](https://docs.microsoft.com/graph/known-issues)

**Gde mogu da proverim status dostupnosti usluge i povezanosti?**

Dostupnost usluge i povezivanje glavnih usluga pristupačnosti putem Microsoft Graph mogu da utiču na ukupnu dostupnost i performanse Microsoft Graph.

- Više Azure Active Directory usluge proverite status usluga **"Bezbednost i identitet"** navedenog na stranici ["Azure status"](https://azure.microsoft.com/status/).
- Ako Kancelarija usluge koje doprinose korporaciji Microsoft Graph, proverite status usluga navedenih na kontrolnoj tabli za [Kancelarija Isveba usluge.](https://portal.office.com/adminportal/home#/servicehealth)

Microsoft Graph greške u autorizovanju mogu biti rezultat nekoliko različitih problema, od kojih većina generiše grešku 401 ili 403. Na primer, sve sledeće može dovesti do grešaka u autorizovanju:

- Neispravno [tokovi prikupljanja tokena za pristup](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-scenarios)
- Loše konfigurisani[opsezi dozvola](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes)
- Nedostatak [pristanka](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent)

***Kraj podrške za Azure Active Directory biblioteke potvrde identiteta (ADAL) i Azure AD Graph API (AAD Graph)***

**Počev od 30. juna 2020.** više nećemo dodavati nove funkcije u ADAL i Azure AD Graph. Nastavićemo da pružamo tehničku podršku i bezbednosne ispravke, ali više nećemo pružati ispravke funkcija.

**Počev od 30. juna 2022,** završićemo podršku za ADAL i Azure AD Graph i više nećemo pružati tehničku podršku ili bezbednosne ispravke.

Aplikacije koje koriste ADAL u postojećim verzijama operativnog sistema nastaviće da rade posle tog vremena, ali neće dobiti tehničku podršku *ili bezbednosne ispravke.*

Aplikacije koje koriste Azure AD Graph nakon tog vremena, možda više neće primati odgovore iz Azure AD Graph krajnje tačke.

**ADAL migracija**

Preporučujemo ažuriranje na [Microsoft Authentication Library (MSAL) ](https://docs.microsoft.com/azure/active-directory/develop/v2-overview)koja ima najnovije funkcije i bezbednosne ispravke.

Ako koristite Microsoft aplikacije, znajte da je Microsoft u procesu migriranje aplikacija u MSAL do kraja roka podrške, obezbeđujući da će imati koristi od tekućih poboljšanja bezbednosti i funkcija MSAL.

1. [Pročitajte najčešća pitanja za ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [Saznajte više o tome kako da migrirate aplikacije na osnovu platforme](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. Ako vam je potrebna pomoć da razumete koje aplikacije koriste ADAL, preporučujemo da pregledate izvorni kôd svih aplikacija i, ako je primenljivo, vašoj dobavljačima ISV usluga ili aplikacija. Microsoft podrška vam takođe može pružiti listu svih aplikacija koje nisu Microsoft ADAL u vašem zakupcu.

**AAD Graph migracija**

Za aplikacije koje koriste Azure AD Graph, pratite uputstva da biste migrirali [Azure AD Graph aplikacije](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview)u Microsoft Graph.

1. [Naša lista za migraciju pruža tačku za početak](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).
2. Vaš portal za registraciju aplikacija Azure prikazuje koje aplikacije koriste AAD Graph. Preporučujemo vam da pregledate sav izvorni kod aplikacija i, ako je primenljivo, kontaktirate bilo koje ISV-ove ili dobavljače aplikacija. Microsoft podrška vam takođe može pružiti listu svih AAD Graph koji se koristi u vašem zakučaru.
3. Da bi vaša aplikacija pristupala podacima u sistemu Microsoft Graph, korisnik ili administrator moraju da im dodele odgovarajuće dozvole putem procesa pristanka. Microsoft [Graph za dozvole](https://docs.microsoft.com/graph/permissions-reference) navodi dozvole povezane sa svakim glavnim skupom Microsoft Graph APU-ja. Takođe pruža uputstva o tome kako da koristite dozvole.
