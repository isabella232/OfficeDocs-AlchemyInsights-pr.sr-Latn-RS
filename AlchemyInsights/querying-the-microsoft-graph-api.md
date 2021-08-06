---
title: Izvršavanje upita za Microsoft Graph API
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
- "7846"
ms.openlocfilehash: eda5d8d1d76d0d87312b1441aeae89d8e250abe0e8b613d4a43fcc2345a6f021
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 08/05/2021
ms.locfileid: "53923253"
---
# <a name="querying-the-microsoft-graph-api"></a>Izvršavanje upita za Microsoft Graph API

Ova tema može da se primeni i na projektante koji još uvek koriste Azure AD Graph API. Međutim, preporučuje  se da koristite Microsoft Graph za sve scenarije direktorijuma, identiteta i upravljanja pristupom.

**Problemi sa potvrdom identiteta ili autorizacije**

- Ako aplikacija ne može da pribavi **tokene** za pozivanje aplikacije Microsoft Graph, izabrati problem sa dobijanjem **tokena** za pristup (potvrda identiteta) microsoft Graph kategoriji da biste dobili specifičnije pomoć i podršku za ovu temu.
- Ako aplikacija dobija **401 ili 403** greške u autorizovanju prilikom pozivanja korporacije Microsoft Graph, izabrati kategoriju Dobijanje pristupa je odbijen **(Autorizacija)** Microsoft Graph API da biste dobili određeniju pomoć i podršku za ovu temu.

**Želim da koristim Microsoft Graph, ali nisam siguran odakle da počnem**

Da biste saznali više o Microsoft Graph, pogledajte:

- [Pregled usluge Microsoft Graph](https://docs.microsoft.com/graph/overview)
- [Pregled upravljanja identitetom i pristupom u programu Microsoft Graph](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [Početak izgradnje Microsoft Graph aplikacija](https://docs.microsoft.com/graph/)
- **Microsoft Graph Explorer** – testiranje Microsoft Graph APIT-ja u zakupca ili demo zakupca

**Želim da koristim Microsoft Graph, ali da li podržava v1.0 AD-je direktorijuma koji su mi potrebni?**

Microsoft Graph je preporučeni API za direktorijum, identitet i upravljanje pristupom. Međutim, postoji još nekoliko razlika između onoga što je moguće u Azure AD Graph i Microsoft Graph. Pregledajte sledeće članke koji ističu najažuarnije razlike da biste pomogli pri izboru:

- [Razlike u tipu resursa između usluge Azure AD Graph i Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [Razlike u svojstvima između usluge Azure AD Graph i Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [Razlike u metodima između Azure AD i Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

**Kada izvršavam upit *za objekat korisnika,* nedostaju mnoga njegova svojstva**

`GET https://graph.microsoft.com/v1.0/users`samo daje 11 svojstava, jer Microsoft Graph automatski bira podrazumevani skup korisničkih *svojstava* koje treba vratiti. Ako su vam potrebna druga *korisnička* svojstva, koristite $select da biste izabrali svojstva koja su vam potrebna za aplikaciju. Prvo isprobajte u **programu Microsoft Graph Explorer.**

**Neke vrednosti svojine korisnika su *bez vrednosti iako* znam da su postavljene**

Najverovatnije objašnjenje je da je aplikaciji dodeljena *dozvola User.ReadBasic.Sve.* To aplikaciji omogućava da čita ograničeni skup korisničkih svojstava, vraćajući sva ostala svojstva kao "null" čak i ako su prethodno postavljena. Pokušajte da dodeli *aplikaciji User.Read.All* permission instead.

Dodatne informacije potražite u [članku Microsoft Graph korisničke dozvole.](https://docs.microsoft.com/graph/permissions-reference#user-permissions)

**Imam problema sa korišćenjem OData parametara upita za filtriranje podataka u zahtevima**

Iako Microsoft Graph podržava širok opseg OData parametara upita, mnoge od tih parametara nisu u potpunosti podržane od strane usluga direktorijuma (resursi koji nasleđuju od *direktorijumaObject)* u programu Microsoft Graph. Ista ograničenja koja su bila prisutna u Azure AD Graph trajati najviše u Microsoft Graph:

1. **Nije podržano:**$count, $search i $filter bez vrednosti *ili* bez *vrednosti*
2. **Nije podržano:**$filter određenim svojstvima (pogledajte teme o resursima na kojima se svojstva mogu filtrirati)
3. **Nije podržano**: stranik, filtriranje i sortiranje u isto vreme
4. **Nije podržano:** filtriranje relacije. Na primer – pronađite sve članove grupe inženjera koji su u UK.
5. **Delimična** podrška: $orderby *korisniku* (samo za displayName i userPrincipalName) i *grupi*
6. **Delimična** podrška: $filter (podržava samo *eq*, *startwith* *ili* *,* i ograničena bilo koja *)* podršku, $expand (proširivanje relacija jednog objekta vraća sve relacije, ali je proširenje kolekcije relacija objekata ograničeno)

Dodatne informacije potražite u [temi Prilagođavanje odgovora parametrima upita.](https://docs.microsoft.com/graph/query-parameters)

**API koji pozivam ne funkcioniše – gde mogu da uradim više testiranja?**

**Microsoft Graph Explorer** – testirajte Microsoft Graph ABE-je u zakupca ili demo  verziji zakupca, a pogledajte i uzorke upita u programu Microsoft Graph Explorer.

**Kada izvršavam upit za podatke, izgleda kao da ponovo dobijam nepotpuni skup podataka**

Ako obavljate upite za kolekciju (kao što su *korisnici),* Microsoft Graph koristi ograničenja stranice na strani servera tako da se rezultati uvek vraćaju sa podrazumevanom veličinom stranice. Aplikacija bi uvek trebalo da očekuje stranice koje se vraćaju iz usluge.

Za više informacija pogledajte:

- [Najbolje Graph Microsoft naloga](https://docs.microsoft.com/graph/best-practices-concept)
- [Paging Microsoft Graph data in your app](https://docs.microsoft.com/graph/paging)

**Moja aplikacija je suviše spora i reaguje. Koja poboljšanja mogu da napravim?**

U zavisnosti od scenarija, na raspolaganju vam je mnoštvo različitih opcija kako biste aplikaciju načinili performativnijim, a u nekim slučajevima manje ćete biti skloni da ih usluga remeti (kada upućujete previše poziva).

Više informacija potražite u sledećim člancima:

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
