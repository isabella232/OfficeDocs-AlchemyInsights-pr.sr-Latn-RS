---
title: Izvršavanje upita prema Microsoft Graph API
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
ms.openlocfilehash: 527e88c7b3cb1cc4f5535e3b0d2bc4d8d1163336
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: sr-Latn-RS
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974684"
---
# <a name="querying-the-microsoft-graph-api"></a>Izvršavanje upita prema Microsoft Graph API

Ova tema može da se primenjuje i na programere koji i dalje koriste Azure AD Graph Graf. Međutim **, preporučuje se** da koristite Microsoft Graph za sve kataloge, identitete i Access scenarije upravljanja pristupom.

**Problemi sa autentikacijom ili autorizacijom**

- Ako aplikacija **ne može da dobije simbole** da bi pozvala Microsoft Graph, odaberite **problem sa prilikom dobijanja simbola za pristup (potvrda identiteta)** Microsoft Graph da bi se pribavila preciznije pomoć i podrška na ovoj temi.
- Ako aplikacija **prima 401 ili 403 greške autorizacije** prilikom pozivanja Microsoft dijagrama, izaberite kategoriju " **Preuzimanje zabrane pristupa" (autorizacija)** Microsoft Graph API za dobijanje specifične pomoći i podrške u ovoj temi.

**Želim da koristim Microsoft Graph, ali ne znam gde da počnem**

Da biste saznali više o programu Microsoft Graph, pogledajte:

- [Pregled programa Microsoft Graph](https://docs.microsoft.com/graph/overview)
- [Pregled identiteta i upravljanja pristupom u programu Microsoft Graph](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [Prvi koraci u pravljenju Microsoft Graph aplikacija](https://docs.microsoft.com/graph/)
- **Microsoft Graph Explorer** – testiranje Microsoft Graph API-ja u zakupcu ili na demo zakupcu

**Želim da koristim Microsoft Graph, ali da li podržava API-ju usluge v 1.0?**

Microsoft Graph je preporučeni API za upravljanje katalogom, identitetom i Access upravljanju. Međutim, postoji nekoliko razmaka između onoga što je moguće u usluzi Azure A.D. i Microsoft Graph. Pregledajte sledeće članke koji naglašavaju najnovije razlike koje će vam pomoći u izboru:

- [Razlike tipa resursa između Azure reklama i Microsoft dijagrama](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [Razlike u svojstvima između Azure A.D. Grafa i Microsoft dijagrama](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [Razlike metoda između Azure AD i Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

**Kada upitim *korisnički* objekat, mnoga svojstva nedostaju**

`GET https://graph.microsoft.com/v1.0/users` daje samo 11 svojstava, kao što Microsoft Graph automatski bira podrazumevani skupa svojstava *korisnika* . Ako su vam potrebna i druga svojstva *korisnika* , koristite $SELECT da biste izabrali svojstva koja su vam potrebna. Prvo isprobajte **Microsoft Graph Explorer** .

**Neke vrednosti korisničkog vlasništva su *Null* iako znam da su podešene**

Najverovatnije objašnjenje je da je aplikaciji dodeljena *Korisnička. ReadBasic. sva* dozvola. To omogućava aplikaciji da čita ograničeni broj svojstava korisnika, vraća sva druga svojstva kao NULL, čak i ako su prethodno podešene. Isprobajte *korisniku aplikacije. pročitajte. sve* dozvole.

Više informacija potražite u članku [dozvole za Microsoft Graph](https://docs.microsoft.com/graph/permissions-reference#user-permissions).

**Imam problema sa korišćenjem OData parametara upita za filtriranje podataka u svojim zahtevima**

Dok Microsoft Graph podržava širok opseg parametara OData upita, mnogi od tih parametara nisu u potpunosti podržani od strane usluga direktorijuma (resursi koji nasleđuju od *Directoryobject*) u programu Microsoft Graph. Ista ograničenja koja su bila prisutan u usluzi Azure AD Graph se i dalje najčešće nalaze u programu Microsoft Graph:

1. **Nije podržano**: $count, $search i $filter u vrednostima *Null* ili *Ne bez* vrednosti
2. **Nije podržano**: $filter na određenim svojstvima (pogledajte teme za resurse na kojima su svojstva filtriena)
3. **Nije podržano**: istovremeno stranične memorije, filtriranje i sortiranje
4. **Nije podržano**: filtriranje relacije. Na primer – pronađite sve članove inženjerske grupe koji se nalaze u Britaniji.
5. **Delimična podrška**: $OrderBy na *korisničkom* (Displayime i userprincipalime) i *grupi*
6. **Delimična podrška**: $filter (podržava samo *EQ*, *startswith*, *ili*, *i* ograničeno *bilo koja*) podrška, $Expand (proširivanje relacija jednog objekta vraća sve relacije, ali proširenje relacija objekata se ograničava)

Više informacija potražite u članku [Prilagođavanje odgovora pomoću parametara upita](https://docs.microsoft.com/graph/query-parameters).

**API koji zovem ne radi-gde mogu da uradim više testiranja?**

**Microsoft Graph Explorer** – testiranje Microsoft Graph API-ja u zakupcu ili na demonstracijuzakupcu i pročitajte **probne upite** u programu Microsoft Graph Explorer.

**Kada upitim za podatke, čini se da dobijam nazad nepotpun skupa podataka**

Ako upitate kolekciju (kao što su *Korisnici*), Microsoft Graph koristi ograničenja stranice servera tako da se rezultati uvek vraćaju sa podrazumevanom veličinom stranice. Aplikacija bi uvek trebalo da očekuje da stranica kroz kolekcije vrati iz usluge.

Za više informacija pogledajte članak:

- [Najbolje prakse za Microsoft Graph](https://docs.microsoft.com/graph/best-practices-concept)
- [Stranične memorije za Microsoft Graph u aplikaciji](https://docs.microsoft.com/graph/paging)

**Moja aplikacija je prespora i takođe se koristi. Koja poboljšanja mogu da napravim?**

U zavisnosti od scenarija, postoji mnoštvo različitih opcija koje su vam na raspolaganju da bi aplikacija bila pristupačnija, a u nekoliko slučajeva, manje sklona odbacivanju od strane usluge (kada pravite previše poziva).

Više informacija potražite u sledećim člancima:

- [Najbolje prakse za Microsoft Graph](https://docs.microsoft.com/graph/best-practices-concept)
- [Zahtevi za sastanak](https://docs.microsoft.com/graph/json-batching)
- [Praćenje promena kroz Delta Query](https://docs.microsoft.com/graph/delta-query-overview)
- [Obaveštenje o promenama pomoću Veb-udica](https://docs.microsoft.com/graph/webhooks)
- [Usmeravanje smernica](https://docs.microsoft.com/graph/throttling)

**Gde mogu da pronađem više informacija o greškama i poznatim problemima?**

- [Informacije o odgovoru na Microsoft Graph](https://docs.microsoft.com/graph/errors)
- [Poznati problemi sa programom Microsoft Graph](https://docs.microsoft.com/graph/known-issues)

**Gde mogu da proverim status raspoloživost usluge i vezu?**

Raspoloživost usluge i veza osnovnih usluga kojima se može pristupiti pomoću programa Microsoft Graph može da utiče na ukupnu dostupnost i performanse programa Microsoft Graph.

- Za Azure Active Directory zdravstveni sistem, potvrdite status **bezbednosti + usluge identiteta** navedenih na [stranici Azure status](https://azure.microsoft.com/status/).
- Za Office usluge koje doprinose programu Microsoft Graph, potvrdite status usluga navedenim na [kontrolnoj tabli usluge Office usluga](https://portal.office.com/adminportal/home#/servicehealth).
